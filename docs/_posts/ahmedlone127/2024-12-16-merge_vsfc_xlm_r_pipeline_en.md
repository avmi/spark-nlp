---
layout: model
title: English merge_vsfc_xlm_r_pipeline pipeline XlmRoBertaForSequenceClassification from ThuyNT03
author: John Snow Labs
name: merge_vsfc_xlm_r_pipeline
date: 2024-12-16
tags: [en, open_source, pipeline, onnx]
task: Text Classification
language: en
edition: Spark NLP 5.5.1
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained XlmRoBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`merge_vsfc_xlm_r_pipeline` is a English model originally trained by ThuyNT03.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/merge_vsfc_xlm_r_pipeline_en_5.5.1_3.0_1734355705156.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/merge_vsfc_xlm_r_pipeline_en_5.5.1_3.0_1734355705156.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("merge_vsfc_xlm_r_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("merge_vsfc_xlm_r_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|merge_vsfc_xlm_r_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.1+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|773.3 MB|

## References

https://huggingface.co/ThuyNT03/Merge_vsfc_XLM-R

## Included Models

- DocumentAssembler
- TokenizerModel
- XlmRoBertaForSequenceClassification