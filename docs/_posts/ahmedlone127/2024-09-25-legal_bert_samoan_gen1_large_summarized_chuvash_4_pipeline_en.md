---
layout: model
title: English legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline pipeline BertForSequenceClassification from wiorz
author: John Snow Labs
name: legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline
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

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline` is a English model originally trained by wiorz.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline_en_5.5.0_3.0_1727288653152.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline_en_5.5.0_3.0_1727288653152.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|legal_bert_samoan_gen1_large_summarized_chuvash_4_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|409.5 MB|

## References

https://huggingface.co/wiorz/legal_bert_sm_gen1_large_summarized_cv_4

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification