---
layout: model
title: None opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline pipeline MarianTransformer from sriram-sanjeev9s
author: John Snow Labs
name: opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline
date: 2024-09-08
tags: [nan, open_source, pipeline, onnx]
task: Translation
language: nan
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained MarianTransformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline` is a None model originally trained by sriram-sanjeev9s.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline_nan_5.5.0_3.0_1725765349182.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline_nan_5.5.0_3.0_1725765349182.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline", lang = "nan")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline", lang = "nan")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|opus_maltese_english_french_wmt14_english_french_1million_20epochs_v2_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|nan|
|Size:|502.5 MB|

## References

https://huggingface.co/sriram-sanjeev9s/opus-mt-en-fr_wmt14_En_Fr_1million_20epochs_v2

## Included Models

- DocumentAssembler
- SentenceDetectorDLModel
- MarianTransformer