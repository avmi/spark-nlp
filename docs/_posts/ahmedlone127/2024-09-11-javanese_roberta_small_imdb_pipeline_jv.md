---
layout: model
title: Javanese javanese_roberta_small_imdb_pipeline pipeline RoBertaEmbeddings from w11wo
author: John Snow Labs
name: javanese_roberta_small_imdb_pipeline
date: 2024-09-11
tags: [jv, open_source, pipeline, onnx]
task: Embeddings
language: jv
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`javanese_roberta_small_imdb_pipeline` is a Javanese model originally trained by w11wo.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/javanese_roberta_small_imdb_pipeline_jv_5.5.0_3.0_1726023991367.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/javanese_roberta_small_imdb_pipeline_jv_5.5.0_3.0_1726023991367.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("javanese_roberta_small_imdb_pipeline", lang = "jv")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("javanese_roberta_small_imdb_pipeline", lang = "jv")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|javanese_roberta_small_imdb_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|jv|
|Size:|465.9 MB|

## References

https://huggingface.co/w11wo/javanese-roberta-small-imdb

## Included Models

- DocumentAssembler
- TokenizerModel
- RoBertaEmbeddings