---
layout: model
title: English toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline pipeline BertForSequenceClassification from l2reg
author: John Snow Labs
name: toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline
date: 2024-09-26
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

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline` is a English model originally trained by l2reg.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline_en_5.5.0_3.0_1727311068189.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline_en_5.5.0_3.0_1727311068189.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|toxic_dbmdz_bert_base_turkish_128k_uncased_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|691.6 MB|

## References

https://huggingface.co/l2reg/toxic-dbmdz-bert-base-turkish-128k-uncased

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification