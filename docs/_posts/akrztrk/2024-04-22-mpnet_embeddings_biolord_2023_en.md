---
layout: model
title: English BioLORD-2023 MPNetEmbeddings from FremyCompany
author: John Snow Labs
name: mpnet_embeddings_biolord_2023
date: 2024-04-22
tags: [mpnet, en, embeddings, biolord, open_source, onnx]
task: Embeddings
language: en
edition: Spark NLP 5.2.2
spark_version: 3.0
supported: true
engine: onnx
annotator: MPNetEmbeddings
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained MPNetEmbeddings model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP `mpnet_embeddings_biolord_2023` is a English model originally trained by `FremyCompany`.

## Predicted Entities



{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/mpnet_embeddings_biolord_2023_en_5.2.2_3.0_1713822166758.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/mpnet_embeddings_biolord_2023_en_5.2.2_3.0_1713822166758.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
document_assembler = DocumentAssembler()\
    .setInputCol("text")\
    .setOutputCol("documents")
    
embeddings =MPNetEmbeddings.pretrained("mpnet_embeddings_biolord_2023","en")\
    .setInputCols(["documents"])\
    .setOutputCol("mpnet_embeddings")

pipeline = Pipeline().setStages([document_assembler, embeddings])

result = pipeline.fit(data).transform(data)
```
```scala
val document_assembler = new DocumentAssembler()
    .setInputCol("text") 
    .setOutputCol("documents")
    
val embeddings = MPNetEmbeddings 
    .pretrained("mpnet_embeddings_biolord_2023", "en")
    .setInputCols(Array("documents")) 
    .setOutputCol("mpnet_embeddings") 

val pipeline = new Pipeline().setStages(Array(document_assembler, embeddings))

val result = pipeline.fit(data).transform(data)
```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|mpnet_embeddings_biolord_2023|
|Compatibility:|Spark NLP 5.2.2+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document]|
|Output Labels:|[MPNet]|
|Language:|en|
|Size:|407.0 MB|

## References

https://huggingface.co/FremyCompany/BioLORD-2023