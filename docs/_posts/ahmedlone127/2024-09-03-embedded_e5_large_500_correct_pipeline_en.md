---
layout: model
title: English embedded_e5_large_500_correct_pipeline pipeline E5Embeddings from rithwik-db
author: John Snow Labs
name: embedded_e5_large_500_correct_pipeline
date: 2024-09-03
tags: [en, open_source, pipeline, onnx]
task: Embeddings
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

Pretrained E5Embeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`embedded_e5_large_500_correct_pipeline` is a English model originally trained by rithwik-db.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/embedded_e5_large_500_correct_pipeline_en_5.5.0_3.0_1725341123045.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/embedded_e5_large_500_correct_pipeline_en_5.5.0_3.0_1725341123045.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("embedded_e5_large_500_correct_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("embedded_e5_large_500_correct_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|embedded_e5_large_500_correct_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|1.2 GB|

## References

https://huggingface.co/rithwik-db/embedded-e5-large-500-correct

## Included Models

- DocumentAssembler
- E5Embeddings