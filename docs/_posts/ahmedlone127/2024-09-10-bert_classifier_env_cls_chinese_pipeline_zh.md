---
layout: model
title: Chinese bert_classifier_env_cls_chinese_pipeline pipeline BertForSequenceClassification from celtics1863
author: John Snow Labs
name: bert_classifier_env_cls_chinese_pipeline
date: 2024-09-10
tags: [zh, open_source, pipeline, onnx]
task: Text Classification
language: zh
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`bert_classifier_env_cls_chinese_pipeline` is a Chinese model originally trained by celtics1863.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bert_classifier_env_cls_chinese_pipeline_zh_5.5.0_3.0_1725957974456.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bert_classifier_env_cls_chinese_pipeline_zh_5.5.0_3.0_1725957974456.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("bert_classifier_env_cls_chinese_pipeline", lang = "zh")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("bert_classifier_env_cls_chinese_pipeline", lang = "zh")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bert_classifier_env_cls_chinese_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|zh|
|Size:|383.5 MB|

## References

https://huggingface.co/celtics1863/env-bert-cls-chinese

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification