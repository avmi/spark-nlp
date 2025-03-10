---
layout: model
title: Akan akan_tiny_2000ms_1k_pipeline pipeline WhisperForCTC from devkyle
author: John Snow Labs
name: akan_tiny_2000ms_1k_pipeline
date: 2024-09-16
tags: [ak, open_source, pipeline, onnx]
task: Automatic Speech Recognition
language: ak
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained WhisperForCTC, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`akan_tiny_2000ms_1k_pipeline` is a Akan model originally trained by devkyle.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/akan_tiny_2000ms_1k_pipeline_ak_5.5.0_3.0_1726476566938.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/akan_tiny_2000ms_1k_pipeline_ak_5.5.0_3.0_1726476566938.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("akan_tiny_2000ms_1k_pipeline", lang = "ak")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("akan_tiny_2000ms_1k_pipeline", lang = "ak")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|akan_tiny_2000ms_1k_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|ak|
|Size:|389.6 MB|

## References

https://huggingface.co/devkyle/Akan-tiny-2000ms-1k

## Included Models

- AudioAssembler
- WhisperForCTC