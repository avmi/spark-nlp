---
layout: model
title: English finetuned_bge_embeddings_v3_base_v1_5_pipeline pipeline BGEEmbeddings from austinpatrickm
author: John Snow Labs
name: finetuned_bge_embeddings_v3_base_v1_5_pipeline
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

Pretrained BGEEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`finetuned_bge_embeddings_v3_base_v1_5_pipeline` is a English model originally trained by austinpatrickm.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/finetuned_bge_embeddings_v3_base_v1_5_pipeline_en_5.5.0_3.0_1725229508197.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/finetuned_bge_embeddings_v3_base_v1_5_pipeline_en_5.5.0_3.0_1725229508197.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("finetuned_bge_embeddings_v3_base_v1_5_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("finetuned_bge_embeddings_v3_base_v1_5_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|finetuned_bge_embeddings_v3_base_v1_5_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|387.1 MB|

## References

https://huggingface.co/austinpatrickm/finetuned_bge_embeddings_v3_base_v1.5

## Included Models

- DocumentAssembler
- BGEEmbeddings