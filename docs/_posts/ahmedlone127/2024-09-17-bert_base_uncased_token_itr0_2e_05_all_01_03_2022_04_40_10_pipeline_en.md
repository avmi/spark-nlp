---
layout: model
title: English bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline pipeline BertForTokenClassification from ali2066
author: John Snow Labs
name: bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline
date: 2024-09-17
tags: [en, open_source, pipeline, onnx]
task: Named Entity Recognition
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

Pretrained BertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline` is a English model originally trained by ali2066.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline_en_5.5.0_3.0_1726608403413.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline_en_5.5.0_3.0_1726608403413.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bert_base_uncased_token_itr0_2e_05_all_01_03_2022_04_40_10_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|407.2 MB|

## References

https://huggingface.co/ali2066/bert-base-uncased_token_itr0_2e-05_all_01_03_2022-04_40_10

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForTokenClassification