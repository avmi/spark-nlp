---
layout: model
title: Central Khmer, Khmer khmer_xlm_roberta_base_pipeline pipeline XlmRoBertaEmbeddings from channudam
author: John Snow Labs
name: khmer_xlm_roberta_base_pipeline
date: 2024-09-03
tags: [km, open_source, pipeline, onnx]
task: Embeddings
language: km
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained XlmRoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`khmer_xlm_roberta_base_pipeline` is a Central Khmer, Khmer model originally trained by channudam.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/khmer_xlm_roberta_base_pipeline_km_5.5.0_3.0_1725391621478.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/khmer_xlm_roberta_base_pipeline_km_5.5.0_3.0_1725391621478.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("khmer_xlm_roberta_base_pipeline", lang = "km")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("khmer_xlm_roberta_base_pipeline", lang = "km")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|khmer_xlm_roberta_base_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|km|
|Size:|1.0 GB|

## References

https://huggingface.co/channudam/khmer-xlm-roberta-base

## Included Models

- DocumentAssembler
- TokenizerModel
- XlmRoBertaEmbeddings