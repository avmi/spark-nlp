---
layout: model
title: Multilingual nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased BertForTokenClassification from GuCuChiara
author: John Snow Labs
name: nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased
date: 2023-11-08
tags: [bert, xx, open_source, token_classification, onnx]
task: Named Entity Recognition
language: xx
edition: Spark NLP 5.2.0
spark_version: 3.0
supported: true
engine: onnx
annotator: BertForTokenClassification
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForTokenClassification model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased` is a Multilingual model originally trained by GuCuChiara.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased_xx_5.2.0_3.0_1699409457516.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased_xx_5.2.0_3.0_1699409457516.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python


documentAssembler = DocumentAssembler() \
    .setInputCol("text") \
    .setOutputCol("documents")
    
    
tokenClassifier = BertForTokenClassification.pretrained("nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased","xx") \
            .setInputCols(["documents","token"]) \
            .setOutputCol("ner")

pipeline = Pipeline().setStages([documentAssembler, tokenClassifier])

pipelineModel = pipeline.fit(data)

pipelineDF = pipelineModel.transform(data)

```
```scala


val documentAssembler = new DocumentAssembler()
    .setInputCol("text") 
    .setOutputCol("embeddings")
    
val tokenClassifier = BertForTokenClassification  
    .pretrained("nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased", "xx")
    .setInputCols(Array("documents","token")) 
    .setOutputCol("ner") 

val pipeline = new Pipeline().setStages(Array(documentAssembler, tokenClassifier))

val pipelineModel = pipeline.fit(data)

val pipelineDF = pipelineModel.transform(data)


```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|nlp_hiba_distemist_fine_tuned_bert_base_multilingual_cased|
|Compatibility:|Spark NLP 5.2.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[documents, token]|
|Output Labels:|[ner]|
|Language:|xx|
|Size:|665.1 MB|

## References

https://huggingface.co/GuCuChiara/NLP-HIBA_DisTEMIST_fine_tuned_bert-base-multilingual-cased