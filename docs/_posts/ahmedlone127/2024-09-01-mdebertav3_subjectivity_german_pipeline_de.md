---
layout: model
title: German mdebertav3_subjectivity_german_pipeline pipeline DeBertaForSequenceClassification from GroNLP
author: John Snow Labs
name: mdebertav3_subjectivity_german_pipeline
date: 2024-09-01
tags: [de, open_source, pipeline, onnx]
task: Text Classification
language: de
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DeBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`mdebertav3_subjectivity_german_pipeline` is a German model originally trained by GroNLP.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/mdebertav3_subjectivity_german_pipeline_de_5.5.0_3.0_1725208838891.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/mdebertav3_subjectivity_german_pipeline_de_5.5.0_3.0_1725208838891.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("mdebertav3_subjectivity_german_pipeline", lang = "de")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("mdebertav3_subjectivity_german_pipeline", lang = "de")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|mdebertav3_subjectivity_german_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|de|
|Size:|860.3 MB|

## References

https://huggingface.co/GroNLP/mdebertav3-subjectivity-german

## Included Models

- DocumentAssembler
- TokenizerModel
- DeBertaForSequenceClassification