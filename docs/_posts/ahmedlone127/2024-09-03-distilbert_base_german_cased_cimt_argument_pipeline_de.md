---
layout: model
title: German distilbert_base_german_cased_cimt_argument_pipeline pipeline DistilBertForSequenceClassification from juliaromberg
author: John Snow Labs
name: distilbert_base_german_cased_cimt_argument_pipeline
date: 2024-09-03
tags: [de, open_source, pipeline, onnx]
task: Text Classification
language: de
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DistilBertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`distilbert_base_german_cased_cimt_argument_pipeline` is a German model originally trained by juliaromberg.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/distilbert_base_german_cased_cimt_argument_pipeline_de_5.5.0_3.0_1725394033991.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/distilbert_base_german_cased_cimt_argument_pipeline_de_5.5.0_3.0_1725394033991.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("distilbert_base_german_cased_cimt_argument_pipeline", lang = "de")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("distilbert_base_german_cased_cimt_argument_pipeline", lang = "de")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|distilbert_base_german_cased_cimt_argument_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|de|
|Size:|252.5 MB|

## References

https://huggingface.co/juliaromberg/distilbert-base-german-cased_cimt-argument

## Included Models

- DocumentAssembler
- TokenizerModel
- DistilBertForSequenceClassification