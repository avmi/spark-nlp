---
layout: model
title: English qa_model2_zhaoxinwind_pipeline pipeline DistilBertForQuestionAnswering from zhaoxinwind
author: John Snow Labs
name: qa_model2_zhaoxinwind_pipeline
date: 2024-09-08
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

Pretrained DistilBertForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`qa_model2_zhaoxinwind_pipeline` is a English model originally trained by zhaoxinwind.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/qa_model2_zhaoxinwind_pipeline_en_5.5.0_3.0_1725818144873.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/qa_model2_zhaoxinwind_pipeline_en_5.5.0_3.0_1725818144873.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("qa_model2_zhaoxinwind_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("qa_model2_zhaoxinwind_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|qa_model2_zhaoxinwind_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|247.3 MB|

## References

https://huggingface.co/zhaoxinwind/QA_model2

## Included Models

- MultiDocumentAssembler
- DistilBertForQuestionAnswering