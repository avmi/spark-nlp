---
layout: model
title: Russian response_quality_classifier_large_pipeline pipeline RoBertaForSequenceClassification from t-bank-ai
author: John Snow Labs
name: response_quality_classifier_large_pipeline
date: 2024-08-31
tags: [ru, open_source, pipeline, onnx]
task: Text Classification
language: ru
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`response_quality_classifier_large_pipeline` is a Russian model originally trained by t-bank-ai.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/response_quality_classifier_large_pipeline_ru_5.4.2_3.0_1725120247314.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/response_quality_classifier_large_pipeline_ru_5.4.2_3.0_1725120247314.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("response_quality_classifier_large_pipeline", lang = "ru")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("response_quality_classifier_large_pipeline", lang = "ru")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|response_quality_classifier_large_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|ru|
|Size:|1.3 GB|

## References

https://huggingface.co/t-bank-ai/response-quality-classifier-large

## Included Models

- DocumentAssembler
- TokenizerModel
- RoBertaForSequenceClassification