---
layout: model
title: Chinese BertForQuestionAnswering model (from hfl)
author: John Snow Labs
name: bert_qa_chinese_pert_base_mrc
date: 2023-11-14
tags: [zh, open_source, question_answering, bert, onnx]
task: Question Answering
language: zh
edition: Spark NLP 5.2.0
spark_version: 3.0
supported: true
engine: onnx
annotator: BertForQuestionAnswering
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained Question Answering model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP. `chinese-pert-base-mrc` is a Chinese model orginally trained by `hfl`.

## Predicted Entities



{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bert_qa_chinese_pert_base_mrc_zh_5.2.0_3.0_1699997205949.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bert_qa_chinese_pert_base_mrc_zh_5.2.0_3.0_1699997205949.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
document_assembler = MultiDocumentAssembler() \ 
.setInputCols(["question", "context"]) \
.setOutputCols(["document_question", "document_context"])

spanClassifier = BertForQuestionAnswering.pretrained("bert_qa_chinese_pert_base_mrc","zh") \
.setInputCols(["document_question", "document_context"]) \
.setOutputCol("answer") \
.setCaseSensitive(True)

pipeline = Pipeline().setStages([
document_assembler,
spanClassifier
])

example = spark.createDataFrame([["What's my name?", "My name is Clara and I live in Berkeley."]]).toDF("question", "context")

result = pipeline.fit(example).transform(example)
```
```scala
val document = new MultiDocumentAssembler()
.setInputCols("question", "context")
.setOutputCols("document_question", "document_context")

val spanClassifier = BertForQuestionAnswering
.pretrained("bert_qa_chinese_pert_base_mrc","zh")
.setInputCols(Array("document_question", "document_context"))
.setOutputCol("answer")
.setCaseSensitive(true)
.setMaxSentenceLength(512)

val pipeline = new Pipeline().setStages(Array(document, spanClassifier))

val example = Seq(
("Where was John Lenon born?", "John Lenon was born in London and lived in Paris. My name is Sarah and I live in London."),
("What's my name?", "My name is Clara and I live in Berkeley."))
.toDF("question", "context")

val result = pipeline.fit(example).transform(example)
```

{:.nlu-block}
```python
import nlu
nlu.load("zh.answer_question.bert.base").predict("""What's my name?|||"My name is Clara and I live in Berkeley.""")
```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bert_qa_chinese_pert_base_mrc|
|Compatibility:|Spark NLP 5.2.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[sentence, token]|
|Output Labels:|[embeddings]|
|Language:|zh|
|Size:|381.1 MB|
|Case sensitive:|true|
|Max sentence length:|512|

## References

References

- https://huggingface.co/hfl/chinese-pert-base-mrc
- https://github.com/ymcui/PERT
- https://github.com/ymcui/Chinese-ELECTRA
- https://github.com/ymcui/Chinese-Minority-PLM
- https://github.com/ymcui/HFL-Anthology
- https://github.com/ymcui/Chinese-BERT-wwm
- https://github.com/ymcui/Chinese-XLNet
- https://github.com/airaria/TextBrewer
- https://github.com/ymcui/MacBERT