---
layout: model
title: English bert_base_uncased_finetuned_bible_pipeline pipeline BertEmbeddings from Pragash-Mohanarajah
author: John Snow Labs
name: bert_base_uncased_finetuned_bible_pipeline
date: 2024-09-19
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

Pretrained BertEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`bert_base_uncased_finetuned_bible_pipeline` is a English model originally trained by Pragash-Mohanarajah.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bert_base_uncased_finetuned_bible_pipeline_en_5.5.0_3.0_1726717677937.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bert_base_uncased_finetuned_bible_pipeline_en_5.5.0_3.0_1726717677937.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("bert_base_uncased_finetuned_bible_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("bert_base_uncased_finetuned_bible_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bert_base_uncased_finetuned_bible_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|407.2 MB|

## References

https://huggingface.co/Pragash-Mohanarajah/bert-base-uncased-finetuned-bible

## Included Models

- DocumentAssembler
- TokenizerModel
- BertEmbeddings