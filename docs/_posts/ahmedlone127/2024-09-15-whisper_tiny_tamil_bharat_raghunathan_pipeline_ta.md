---
layout: model
title: Tamil whisper_tiny_tamil_bharat_raghunathan_pipeline pipeline WhisperForCTC from bharat-raghunathan
author: John Snow Labs
name: whisper_tiny_tamil_bharat_raghunathan_pipeline
date: 2024-09-15
tags: [ta, open_source, pipeline, onnx]
task: Automatic Speech Recognition
language: ta
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained WhisperForCTC, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`whisper_tiny_tamil_bharat_raghunathan_pipeline` is a Tamil model originally trained by bharat-raghunathan.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/whisper_tiny_tamil_bharat_raghunathan_pipeline_ta_5.5.0_3.0_1726426518626.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/whisper_tiny_tamil_bharat_raghunathan_pipeline_ta_5.5.0_3.0_1726426518626.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("whisper_tiny_tamil_bharat_raghunathan_pipeline", lang = "ta")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("whisper_tiny_tamil_bharat_raghunathan_pipeline", lang = "ta")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|whisper_tiny_tamil_bharat_raghunathan_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|ta|
|Size:|390.9 MB|

## References

https://huggingface.co/bharat-raghunathan/whisper-tiny-ta

## Included Models

- AudioAssembler
- WhisperForCTC