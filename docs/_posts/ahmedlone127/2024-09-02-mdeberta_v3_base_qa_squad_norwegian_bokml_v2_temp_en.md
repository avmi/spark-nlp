---
layout: model
title: English mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp DeBertaForQuestionAnswering from eanderson
author: John Snow Labs
name: mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp
date: 2024-09-02
tags: [en, open_source, onnx, question_answering, deberta]
task: Question Answering
language: en
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
engine: onnx
annotator: DeBertaForQuestionAnswering
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DeBertaForQuestionAnswering model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp` is a English model originally trained by eanderson.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp_en_5.5.0_3.0_1725268879818.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp_en_5.5.0_3.0_1725268879818.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
             
documentAssembler = MultiDocumentAssembler() \
     .setInputCol(["question", "context"]) \
     .setOutputCol(["document_question", "document_context"])
    
spanClassifier = DeBertaForQuestionAnswering.pretrained("mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp","en") \
     .setInputCols(["document_question","document_context"]) \
     .setOutputCol("answer")

pipeline = Pipeline().setStages([documentAssembler, spanClassifier])
data = spark.createDataFrame([["What framework do I use?","I use spark-nlp."]]).toDF("document_question", "document_context")
pipelineModel = pipeline.fit(data)
pipelineDF = pipelineModel.transform(data)

```
```scala

val documentAssembler = new MultiDocumentAssembler()
    .setInputCol(Array("question", "context")) 
    .setOutputCol(Array("document_question", "document_context"))
    
val spanClassifier = DeBertaForQuestionAnswering.pretrained("mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp", "en")
    .setInputCols(Array("document_question","document_context")) 
    .setOutputCol("answer") 
    
val pipeline = new Pipeline().setStages(Array(documentAssembler, spanClassifier))
val data = Seq("What framework do I use?","I use spark-nlp.").toDS.toDF("document_question", "document_context")
val pipelineModel = pipeline.fit(data)
val pipelineDF = pipelineModel.transform(data)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|mdeberta_v3_base_qa_squad_norwegian_bokml_v2_temp|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document_question, document_context]|
|Output Labels:|[answer]|
|Language:|en|
|Size:|874.2 MB|

## References

https://huggingface.co/eanderson/mdeberta-v3-base-qa-squad-nb_v2_temp