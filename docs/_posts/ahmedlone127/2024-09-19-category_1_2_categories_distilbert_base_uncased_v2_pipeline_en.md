---
layout: model
title: English category_1_2_categories_distilbert_base_uncased_v2_pipeline pipeline DistilBertForSequenceClassification from chuuhtetnaing
author: John Snow Labs
name: category_1_2_categories_distilbert_base_uncased_v2_pipeline
date: 2024-09-19
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

Pretrained DistilBertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`category_1_2_categories_distilbert_base_uncased_v2_pipeline` is a English model originally trained by chuuhtetnaing.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/category_1_2_categories_distilbert_base_uncased_v2_pipeline_en_5.5.0_3.0_1726744172456.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/category_1_2_categories_distilbert_base_uncased_v2_pipeline_en_5.5.0_3.0_1726744172456.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("category_1_2_categories_distilbert_base_uncased_v2_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("category_1_2_categories_distilbert_base_uncased_v2_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|category_1_2_categories_distilbert_base_uncased_v2_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|249.5 MB|

## References

https://huggingface.co/chuuhtetnaing/category-1-2-categories-distilbert-base-uncased-v2

## Included Models

- DocumentAssembler
- TokenizerModel
- DistilBertForSequenceClassification