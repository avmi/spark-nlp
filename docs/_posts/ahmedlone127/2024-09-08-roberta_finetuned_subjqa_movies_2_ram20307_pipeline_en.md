---
layout: model
title: English roberta_finetuned_subjqa_movies_2_ram20307_pipeline pipeline RoBertaForQuestionAnswering from Ram20307
author: John Snow Labs
name: roberta_finetuned_subjqa_movies_2_ram20307_pipeline
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

Pretrained RoBertaForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`roberta_finetuned_subjqa_movies_2_ram20307_pipeline` is a English model originally trained by Ram20307.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/roberta_finetuned_subjqa_movies_2_ram20307_pipeline_en_5.5.0_3.0_1725758133096.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/roberta_finetuned_subjqa_movies_2_ram20307_pipeline_en_5.5.0_3.0_1725758133096.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("roberta_finetuned_subjqa_movies_2_ram20307_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("roberta_finetuned_subjqa_movies_2_ram20307_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|roberta_finetuned_subjqa_movies_2_ram20307_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|464.1 MB|

## References

https://huggingface.co/Ram20307/roberta-finetuned-subjqa-movies_2

## Included Models

- MultiDocumentAssembler
- RoBertaForQuestionAnswering