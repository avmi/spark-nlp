---
layout: model
title: English further_base_v4_0__checkpoint_last_pipeline pipeline RoBertaEmbeddings from eduagarcia-temp
author: John Snow Labs
name: further_base_v4_0__checkpoint_last_pipeline
date: 2024-09-16
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

Pretrained RoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`further_base_v4_0__checkpoint_last_pipeline` is a English model originally trained by eduagarcia-temp.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/further_base_v4_0__checkpoint_last_pipeline_en_5.5.0_3.0_1726513688044.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/further_base_v4_0__checkpoint_last_pipeline_en_5.5.0_3.0_1726513688044.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("further_base_v4_0__checkpoint_last_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("further_base_v4_0__checkpoint_last_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|further_base_v4_0__checkpoint_last_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|296.3 MB|

## References

https://huggingface.co/eduagarcia-temp/further_base_v4_0__checkpoint_last

## Included Models

- DocumentAssembler
- TokenizerModel
- RoBertaEmbeddings