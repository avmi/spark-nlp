---
layout: model
title: Hebrew whisper_tiny_hebrew_modern_2_mike249_pipeline pipeline WhisperForCTC from mike249
author: John Snow Labs
name: whisper_tiny_hebrew_modern_2_mike249_pipeline
date: 2024-09-15
tags: [he, open_source, pipeline, onnx]
task: Automatic Speech Recognition
language: he
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained WhisperForCTC, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`whisper_tiny_hebrew_modern_2_mike249_pipeline` is a Hebrew model originally trained by mike249.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/whisper_tiny_hebrew_modern_2_mike249_pipeline_he_5.5.0_3.0_1726386999871.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/whisper_tiny_hebrew_modern_2_mike249_pipeline_he_5.5.0_3.0_1726386999871.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("whisper_tiny_hebrew_modern_2_mike249_pipeline", lang = "he")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("whisper_tiny_hebrew_modern_2_mike249_pipeline", lang = "he")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|whisper_tiny_hebrew_modern_2_mike249_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|he|
|Size:|390.1 MB|

## References

https://huggingface.co/mike249/whisper-tiny-he-2

## Included Models

- AudioAssembler
- WhisperForCTC