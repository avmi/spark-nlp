---
layout: model
title: Dhivehi, Divehi, Maldivian hfa_whisper_tiny_divehi_pipeline pipeline WhisperForCTC from kurianbenoy
author: John Snow Labs
name: hfa_whisper_tiny_divehi_pipeline
date: 2024-09-15
tags: [dv, open_source, pipeline, onnx]
task: Automatic Speech Recognition
language: dv
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained WhisperForCTC, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`hfa_whisper_tiny_divehi_pipeline` is a Dhivehi, Divehi, Maldivian model originally trained by kurianbenoy.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/hfa_whisper_tiny_divehi_pipeline_dv_5.5.0_3.0_1726427418594.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/hfa_whisper_tiny_divehi_pipeline_dv_5.5.0_3.0_1726427418594.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("hfa_whisper_tiny_divehi_pipeline", lang = "dv")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("hfa_whisper_tiny_divehi_pipeline", lang = "dv")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|hfa_whisper_tiny_divehi_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|dv|
|Size:|391.3 MB|

## References

https://huggingface.co/kurianbenoy/hfa-whisper-tiny-dv

## Included Models

- AudioAssembler
- WhisperForCTC