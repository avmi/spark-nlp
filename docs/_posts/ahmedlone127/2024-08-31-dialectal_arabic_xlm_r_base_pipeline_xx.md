---
layout: model
title: Multilingual dialectal_arabic_xlm_r_base_pipeline pipeline XlmRoBertaEmbeddings from 3ebdola
author: John Snow Labs
name: dialectal_arabic_xlm_r_base_pipeline
date: 2024-08-31
tags: [xx, open_source, pipeline, onnx]
task: Embeddings
language: xx
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained XlmRoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`dialectal_arabic_xlm_r_base_pipeline` is a Multilingual model originally trained by 3ebdola.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/dialectal_arabic_xlm_r_base_pipeline_xx_5.4.2_3.0_1725126678632.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/dialectal_arabic_xlm_r_base_pipeline_xx_5.4.2_3.0_1725126678632.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("dialectal_arabic_xlm_r_base_pipeline", lang = "xx")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("dialectal_arabic_xlm_r_base_pipeline", lang = "xx")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|dialectal_arabic_xlm_r_base_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|xx|
|Size:|1.0 GB|

## References

https://huggingface.co/3ebdola/Dialectal-Arabic-XLM-R-Base

## Included Models

- DocumentAssembler
- TokenizerModel
- XlmRoBertaEmbeddings