---
layout: model
title: Vietnamese vietnamese_poem_classifier_pipeline pipeline BertForSequenceClassification from Anshler
author: John Snow Labs
name: vietnamese_poem_classifier_pipeline
date: 2024-09-27
tags: [vi, open_source, pipeline, onnx]
task: Text Classification
language: vi
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`vietnamese_poem_classifier_pipeline` is a Vietnamese model originally trained by Anshler.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/vietnamese_poem_classifier_pipeline_vi_5.5.0_3.0_1727404816824.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/vietnamese_poem_classifier_pipeline_vi_5.5.0_3.0_1727404816824.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("vietnamese_poem_classifier_pipeline", lang = "vi")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("vietnamese_poem_classifier_pipeline", lang = "vi")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|vietnamese_poem_classifier_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|vi|
|Size:|414.5 MB|

## References

https://huggingface.co/Anshler/vietnamese-poem-classifier

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification