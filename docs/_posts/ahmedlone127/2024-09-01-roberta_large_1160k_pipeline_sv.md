---
layout: model
title: Swedish roberta_large_1160k_pipeline pipeline RoBertaEmbeddings from AI-Sweden-Models
author: John Snow Labs
name: roberta_large_1160k_pipeline
date: 2024-09-01
tags: [sv, open_source, pipeline, onnx]
task: Embeddings
language: sv
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`roberta_large_1160k_pipeline` is a Swedish model originally trained by AI-Sweden-Models.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/roberta_large_1160k_pipeline_sv_5.4.2_3.0_1725186923941.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/roberta_large_1160k_pipeline_sv_5.4.2_3.0_1725186923941.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("roberta_large_1160k_pipeline", lang = "sv")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("roberta_large_1160k_pipeline", lang = "sv")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|roberta_large_1160k_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|sv|
|Size:|1.3 GB|

## References

https://huggingface.co/AI-Sweden-Models/roberta-large-1160k

## Included Models

- DocumentAssembler
- TokenizerModel
- RoBertaEmbeddings