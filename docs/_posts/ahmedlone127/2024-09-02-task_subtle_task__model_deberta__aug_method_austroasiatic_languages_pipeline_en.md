---
layout: model
title: English task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline pipeline DeBertaForSequenceClassification from BenjaminOcampo
author: John Snow Labs
name: task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline
date: 2024-09-02
tags: [en, open_source, pipeline, onnx]
task: Text Classification
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

Pretrained DeBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline` is a English model originally trained by BenjaminOcampo.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline_en_5.5.0_3.0_1725281641321.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline_en_5.5.0_3.0_1725281641321.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|task_subtle_task__model_deberta__aug_method_austroasiatic_languages_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|607.5 MB|

## References

https://huggingface.co/BenjaminOcampo/task-subtle_task__model-deberta__aug_method-aav

## Included Models

- DocumentAssembler
- TokenizerModel
- DeBertaForSequenceClassification