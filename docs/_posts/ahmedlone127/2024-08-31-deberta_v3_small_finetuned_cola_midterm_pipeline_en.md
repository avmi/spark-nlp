---
layout: model
title: English deberta_v3_small_finetuned_cola_midterm_pipeline pipeline DeBertaForSequenceClassification from kbberendsen
author: John Snow Labs
name: deberta_v3_small_finetuned_cola_midterm_pipeline
date: 2024-08-31
tags: [en, open_source, pipeline, onnx]
task: Text Classification
language: en
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DeBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`deberta_v3_small_finetuned_cola_midterm_pipeline` is a English model originally trained by kbberendsen.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/deberta_v3_small_finetuned_cola_midterm_pipeline_en_5.4.2_3.0_1725124844791.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/deberta_v3_small_finetuned_cola_midterm_pipeline_en_5.4.2_3.0_1725124844791.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("deberta_v3_small_finetuned_cola_midterm_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("deberta_v3_small_finetuned_cola_midterm_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|deberta_v3_small_finetuned_cola_midterm_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|416.2 MB|

## References

https://huggingface.co/kbberendsen/deberta-v3-small-finetuned-cola-midterm

## Included Models

- DocumentAssembler
- TokenizerModel
- DeBertaForSequenceClassification