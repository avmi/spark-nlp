---
layout: model
title: Norwegian Bokmål bert_classifier_norwegian_bokml_large_user_needs_pipeline pipeline BertForSequenceClassification from thusken
author: John Snow Labs
name: bert_classifier_norwegian_bokml_large_user_needs_pipeline
date: 2024-09-09
tags: [nb, open_source, pipeline, onnx]
task: Text Classification
language: nb
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`bert_classifier_norwegian_bokml_large_user_needs_pipeline` is a Norwegian Bokmål model originally trained by thusken.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bert_classifier_norwegian_bokml_large_user_needs_pipeline_nb_5.5.0_3.0_1725900362371.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bert_classifier_norwegian_bokml_large_user_needs_pipeline_nb_5.5.0_3.0_1725900362371.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("bert_classifier_norwegian_bokml_large_user_needs_pipeline", lang = "nb")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("bert_classifier_norwegian_bokml_large_user_needs_pipeline", lang = "nb")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bert_classifier_norwegian_bokml_large_user_needs_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|nb|
|Size:|1.3 GB|

## References

https://huggingface.co/thusken/nb-bert-large-user-needs

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification