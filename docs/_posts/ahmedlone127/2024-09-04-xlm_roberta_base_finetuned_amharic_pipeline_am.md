---
layout: model
title: Amharic xlm_roberta_base_finetuned_amharic_pipeline pipeline XlmRoBertaEmbeddings from Davlan
author: John Snow Labs
name: xlm_roberta_base_finetuned_amharic_pipeline
date: 2024-09-04
tags: [am, open_source, pipeline, onnx]
task: Embeddings
language: am
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained XlmRoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`xlm_roberta_base_finetuned_amharic_pipeline` is a Amharic model originally trained by Davlan.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/xlm_roberta_base_finetuned_amharic_pipeline_am_5.5.0_3.0_1725416891066.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/xlm_roberta_base_finetuned_amharic_pipeline_am_5.5.0_3.0_1725416891066.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("xlm_roberta_base_finetuned_amharic_pipeline", lang = "am")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("xlm_roberta_base_finetuned_amharic_pipeline", lang = "am")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|xlm_roberta_base_finetuned_amharic_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|am|
|Size:|1.0 GB|

## References

https://huggingface.co/Davlan/xlm-roberta-base-finetuned-amharic

## Included Models

- DocumentAssembler
- TokenizerModel
- XlmRoBertaEmbeddings