---
layout: model
title: English ikitracs_conditional MPNetEmbeddings from ilaria-oneofftech
author: John Snow Labs
name: ikitracs_conditional
date: 2024-08-31
tags: [mpnet, en, open_source, onnx]
task: Embeddings
language: en
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
engine: onnx
annotator: MPNetForSequenceClassification
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained MPNetEmbeddings  model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`ikitracs_conditional` is a English model originally trained by ilaria-oneofftech.

## Predicted Entities



{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/ikitracs_conditional_en_5.4.2_3.0_1725145491980.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/ikitracs_conditional_en_5.4.2_3.0_1725145491980.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
document_assembler = DocumentAssembler() \
    .setInputCol("text") \
    .setOutputCol("documents")
    
    
embeddings =MPNetEmbeddings.pretrained("ikitracs_conditional","en") \
            .setInputCols(["documents"]) \
            .setOutputCol("mpnet_embeddings")

pipeline = Pipeline().setStages([document_assembler, embeddings])

pipelineModel = pipeline.fit(data)

pipelineDF = pipelineModel.transform(data)
```
```scala
val document_assembler = new DocumentAssembler()
    .setInputCol("text") 
    .setOutputCol("documents")
    
val embeddings = MPNetEmbeddings 
    .pretrained("ikitracs_conditional", "en")
    .setInputCols(Array("documents")) 
    .setOutputCol("mpnet_embeddings") 

val pipeline = new Pipeline().setStages(Array(document_assembler, embeddings))

val pipelineModel = pipeline.fit(data)

val pipelineDF = pipelineModel.transform(data)
```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|ikitracs_conditional|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document, token]|
|Output Labels:|[class]|
|Language:|en|
|Size:|409.5 MB|

## References

References

https://huggingface.co/ilaria-oneofftech/ikitracs_conditional