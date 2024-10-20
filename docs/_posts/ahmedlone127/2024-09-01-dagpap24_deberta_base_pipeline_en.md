---
layout: model
title: English dagpap24_deberta_base_pipeline pipeline DeBertaEmbeddings from swimmingcrab
author: John Snow Labs
name: dagpap24_deberta_base_pipeline
date: 2024-09-01
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

Pretrained DeBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`dagpap24_deberta_base_pipeline` is a English model originally trained by swimmingcrab.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/dagpap24_deberta_base_pipeline_en_5.5.0_3.0_1725229877500.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/dagpap24_deberta_base_pipeline_en_5.5.0_3.0_1725229877500.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("dagpap24_deberta_base_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("dagpap24_deberta_base_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|dagpap24_deberta_base_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|660.5 MB|

## References

https://huggingface.co/swimmingcrab/DAGPap24-deberta-base

## Included Models

- DocumentAssembler
- TokenizerModel
- DeBertaEmbeddings