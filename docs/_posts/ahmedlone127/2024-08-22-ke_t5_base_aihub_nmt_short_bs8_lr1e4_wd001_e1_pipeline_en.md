---
layout: model
title: English ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline pipeline T5Transformer from datasciathlete
author: John Snow Labs
name: ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline
date: 2024-08-22
tags: [en, open_source, pipeline, onnx]
task: [Question Answering, Summarization, Translation, Text Generation]
language: en
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained T5Transformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline` is a English model originally trained by datasciathlete.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline_en_5.4.2_3.0_1724310045584.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline_en_5.4.2_3.0_1724310045584.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|ke_t5_base_aihub_nmt_short_bs8_lr1e4_wd001_e1_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|1.3 GB|

## References

https://huggingface.co/datasciathlete/ke-t5-base-aihub-nmt-short-bs8-lr1e4-wd001-e1

## Included Models

- DocumentAssembler
- T5Transformer