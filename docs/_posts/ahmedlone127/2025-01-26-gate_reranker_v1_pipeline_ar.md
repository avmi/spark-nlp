---
layout: model
title: Arabic gate_reranker_v1_pipeline pipeline BertForSequenceClassification from NAMAA-Space
author: John Snow Labs
name: gate_reranker_v1_pipeline
date: 2025-01-26
tags: [ar, open_source, pipeline, onnx]
task: Text Classification
language: ar
edition: Spark NLP 5.5.1
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`gate_reranker_v1_pipeline` is a Arabic model originally trained by NAMAA-Space.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/gate_reranker_v1_pipeline_ar_5.5.1_3.0_1737921229288.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/gate_reranker_v1_pipeline_ar_5.5.1_3.0_1737921229288.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("gate_reranker_v1_pipeline", lang = "ar")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("gate_reranker_v1_pipeline", lang = "ar")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|gate_reranker_v1_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.1+|
|License:|Open Source|
|Edition:|Official|
|Language:|ar|
|Size:|507.3 MB|

## References

https://huggingface.co/NAMAA-Space/GATE-Reranker-V1

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification