---
layout: model
title: English finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner RoBertaForTokenClassification from manucos
author: John Snow Labs
name: finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner
date: 2024-09-23
tags: [en, open_source, onnx, token_classification, roberta, ner]
task: Named Entity Recognition
language: en
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
engine: onnx
annotator: RoBertaForTokenClassification
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaForTokenClassification model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner` is a English model originally trained by manucos.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner_en_5.5.0_3.0_1727081601983.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner_en_5.5.0_3.0_1727081601983.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
     
documentAssembler = DocumentAssembler() \
    .setInputCol('text') \
    .setOutputCol('document')
    
tokenizer = Tokenizer() \
    .setInputCols(['document']) \
    .setOutputCol('token')

tokenClassifier  = RoBertaForTokenClassification.pretrained("finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner","en") \
     .setInputCols(["documents","token"]) \
     .setOutputCol("ner")

pipeline = Pipeline().setStages([documentAssembler, tokenizer, tokenClassifier])
data = spark.createDataFrame([["I love spark-nlp"]]).toDF("text")
pipelineModel = pipeline.fit(data)
pipelineDF = pipelineModel.transform(data)

```
```scala

val documentAssembler = new DocumentAssembler()
    .setInputCols("text")
    .setOutputCols("document")
    
val tokenizer = new Tokenizer()
    .setInputCols("document")
    .setOutputCol("token")

val tokenClassifier = RoBertaForTokenClassification.pretrained("finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner", "en")
    .setInputCols(Array("documents","token")) 
    .setOutputCol("ner") 
    
val pipeline = new Pipeline().setStages(Array(documentAssembler, tokenizer, tokenClassifier))
val data = Seq("I love spark-nlp").toDS.toDF("text")
val pipelineModel = pipeline.fit(data)
val pipelineDF = pipelineModel.transform(data)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|finetuned__roberta_clinical_wl_spanish__augmented_ultrasounds_ner|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document, token]|
|Output Labels:|[ner]|
|Language:|en|
|Size:|469.7 MB|

## References

https://huggingface.co/manucos/finetuned__roberta-clinical-wl-es__augmented-ultrasounds-ner