---
layout: model
title: English cnec_2_0_czert_b_base_cased_pipeline pipeline BertForTokenClassification from stulcrad
author: John Snow Labs
name: cnec_2_0_czert_b_base_cased_pipeline
date: 2024-09-14
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

Pretrained BertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`cnec_2_0_czert_b_base_cased_pipeline` is a English model originally trained by stulcrad.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/cnec_2_0_czert_b_base_cased_pipeline_en_5.5.0_3.0_1726306127760.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/cnec_2_0_czert_b_base_cased_pipeline_en_5.5.0_3.0_1726306127760.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("cnec_2_0_czert_b_base_cased_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("cnec_2_0_czert_b_base_cased_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|cnec_2_0_czert_b_base_cased_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|408.6 MB|

## References

https://huggingface.co/stulcrad/CNEC_2_0_Czert-B-base-cased

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForTokenClassification