---
layout: model
title: Catalan, Valencian whisper_base_catalan_pipeline pipeline WhisperForCTC from zuazo
author: John Snow Labs
name: whisper_base_catalan_pipeline
date: 2024-09-17
tags: [ca, open_source, pipeline, onnx]
task: Automatic Speech Recognition
language: ca
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained WhisperForCTC, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`whisper_base_catalan_pipeline` is a Catalan, Valencian model originally trained by zuazo.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/whisper_base_catalan_pipeline_ca_5.5.0_3.0_1726542784525.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/whisper_base_catalan_pipeline_ca_5.5.0_3.0_1726542784525.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("whisper_base_catalan_pipeline", lang = "ca")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("whisper_base_catalan_pipeline", lang = "ca")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|whisper_base_catalan_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|ca|
|Size:|642.8 MB|

## References

https://huggingface.co/zuazo/whisper-base-ca

## Included Models

- AudioAssembler
- WhisperForCTC