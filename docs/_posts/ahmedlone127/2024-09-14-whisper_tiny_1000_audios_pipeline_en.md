---
layout: model
title: English whisper_tiny_1000_audios_pipeline pipeline WhisperForCTC from breco
author: John Snow Labs
name: whisper_tiny_1000_audios_pipeline
date: 2024-09-14
tags: [en, open_source, pipeline, onnx]
task: Automatic Speech Recognition
language: en
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained WhisperForCTC, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`whisper_tiny_1000_audios_pipeline` is a English model originally trained by breco.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/whisper_tiny_1000_audios_pipeline_en_5.5.0_3.0_1726355280211.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/whisper_tiny_1000_audios_pipeline_en_5.5.0_3.0_1726355280211.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("whisper_tiny_1000_audios_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("whisper_tiny_1000_audios_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|whisper_tiny_1000_audios_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|390.0 MB|

## References

https://huggingface.co/breco/whisper-tiny-1000-audios

## Included Models

- AudioAssembler
- WhisperForCTC