---
layout: model
title: English mdeberta_webis_pipeline pipeline DeBertaForQuestionAnswering from intanm
author: John Snow Labs
name: mdeberta_webis_pipeline
date: 2024-09-02
tags: [en, open_source, pipeline, onnx]
task: Question Answering
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

Pretrained DeBertaForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`mdeberta_webis_pipeline` is a English model originally trained by intanm.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/mdeberta_webis_pipeline_en_5.5.0_3.0_1725269387141.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/mdeberta_webis_pipeline_en_5.5.0_3.0_1725269387141.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("mdeberta_webis_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("mdeberta_webis_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|mdeberta_webis_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|849.6 MB|

## References

https://huggingface.co/intanm/mdeberta-webis

## Included Models

- MultiDocumentAssembler
- DeBertaForQuestionAnswering