---
layout: model
title: English ad_kd_bert_base_uncased_qqp_pipeline pipeline BertForSequenceClassification from Brucewsy
author: John Snow Labs
name: ad_kd_bert_base_uncased_qqp_pipeline
date: 2024-09-25
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

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`ad_kd_bert_base_uncased_qqp_pipeline` is a English model originally trained by Brucewsy.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/ad_kd_bert_base_uncased_qqp_pipeline_en_5.5.0_3.0_1727291333754.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/ad_kd_bert_base_uncased_qqp_pipeline_en_5.5.0_3.0_1727291333754.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("ad_kd_bert_base_uncased_qqp_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("ad_kd_bert_base_uncased_qqp_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|ad_kd_bert_base_uncased_qqp_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|409.4 MB|

## References

https://huggingface.co/Brucewsy/AD-KD_bert_base_uncased_qqp

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification