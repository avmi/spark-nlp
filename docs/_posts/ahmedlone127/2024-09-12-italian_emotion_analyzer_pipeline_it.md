---
layout: model
title: Italian italian_emotion_analyzer_pipeline pipeline BertForSequenceClassification from aiknowyou
author: John Snow Labs
name: italian_emotion_analyzer_pipeline
date: 2024-09-12
tags: [it, open_source, pipeline, onnx]
task: Text Classification
language: it
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`italian_emotion_analyzer_pipeline` is a Italian model originally trained by aiknowyou.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/italian_emotion_analyzer_pipeline_it_5.5.0_3.0_1726104528868.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/italian_emotion_analyzer_pipeline_it_5.5.0_3.0_1726104528868.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("italian_emotion_analyzer_pipeline", lang = "it")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("italian_emotion_analyzer_pipeline", lang = "it")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|italian_emotion_analyzer_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|it|
|Size:|412.0 MB|

## References

https://huggingface.co/aiknowyou/it-emotion-analyzer

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification