---
layout: model
title: Multilingual mdeberta_v3_base_triplet_critic_xnli_pipeline pipeline DeBertaForSequenceClassification from Babelscape
author: John Snow Labs
name: mdeberta_v3_base_triplet_critic_xnli_pipeline
date: 2024-09-05
tags: [xx, open_source, pipeline, onnx]
task: Text Classification
language: xx
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DeBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`mdeberta_v3_base_triplet_critic_xnli_pipeline` is a Multilingual model originally trained by Babelscape.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/mdeberta_v3_base_triplet_critic_xnli_pipeline_xx_5.5.0_3.0_1725561952627.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/mdeberta_v3_base_triplet_critic_xnli_pipeline_xx_5.5.0_3.0_1725561952627.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("mdeberta_v3_base_triplet_critic_xnli_pipeline", lang = "xx")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("mdeberta_v3_base_triplet_critic_xnli_pipeline", lang = "xx")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|mdeberta_v3_base_triplet_critic_xnli_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|xx|
|Size:|907.5 MB|

## References

https://huggingface.co/Babelscape/mdeberta-v3-base-triplet-critic-xnli

## Included Models

- DocumentAssembler
- TokenizerModel
- DeBertaForSequenceClassification