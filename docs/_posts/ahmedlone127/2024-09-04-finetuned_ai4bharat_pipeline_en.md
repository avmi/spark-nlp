---
layout: model
title: English finetuned_ai4bharat_pipeline pipeline AlbertEmbeddings from anujsahani01
author: John Snow Labs
name: finetuned_ai4bharat_pipeline
date: 2024-09-04
tags: [en, open_source, pipeline, onnx]
task: Embeddings
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

Pretrained AlbertEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`finetuned_ai4bharat_pipeline` is a English model originally trained by anujsahani01.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/finetuned_ai4bharat_pipeline_en_5.5.0_3.0_1725435559940.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/finetuned_ai4bharat_pipeline_en_5.5.0_3.0_1725435559940.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("finetuned_ai4bharat_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("finetuned_ai4bharat_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|finetuned_ai4bharat_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|125.5 MB|

## References

https://huggingface.co/anujsahani01/finetuned_AI4Bharat

## Included Models

- DocumentAssembler
- TokenizerModel
- AlbertEmbeddings