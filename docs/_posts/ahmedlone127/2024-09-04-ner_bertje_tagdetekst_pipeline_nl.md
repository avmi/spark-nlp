---
layout: model
title: Dutch, Flemish ner_bertje_tagdetekst_pipeline pipeline BertForTokenClassification from surferfelix
author: John Snow Labs
name: ner_bertje_tagdetekst_pipeline
date: 2024-09-04
tags: [nl, open_source, pipeline, onnx]
task: Named Entity Recognition
language: nl
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`ner_bertje_tagdetekst_pipeline` is a Dutch, Flemish model originally trained by surferfelix.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/ner_bertje_tagdetekst_pipeline_nl_5.5.0_3.0_1725477845476.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/ner_bertje_tagdetekst_pipeline_nl_5.5.0_3.0_1725477845476.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("ner_bertje_tagdetekst_pipeline", lang = "nl")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("ner_bertje_tagdetekst_pipeline", lang = "nl")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|ner_bertje_tagdetekst_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|nl|
|Size:|406.8 MB|

## References

https://huggingface.co/surferfelix/ner-bertje-tagdetekst

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForTokenClassification