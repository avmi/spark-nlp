---
layout: model
title: English bge_base_english_v1_5_klej_dyk_pipeline pipeline BGEEmbeddings from ve88ifz2
author: John Snow Labs
name: bge_base_english_v1_5_klej_dyk_pipeline
date: 2024-09-02
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

Pretrained BGEEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`bge_base_english_v1_5_klej_dyk_pipeline` is a English model originally trained by ve88ifz2.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bge_base_english_v1_5_klej_dyk_pipeline_en_5.5.0_3.0_1725241984605.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bge_base_english_v1_5_klej_dyk_pipeline_en_5.5.0_3.0_1725241984605.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("bge_base_english_v1_5_klej_dyk_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("bge_base_english_v1_5_klej_dyk_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bge_base_english_v1_5_klej_dyk_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|385.5 MB|

## References

https://huggingface.co/ve88ifz2/bge-base-en-v1.5-klej-dyk

## Included Models

- DocumentAssembler
- BGEEmbeddings