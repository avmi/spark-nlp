---
layout: model
title: Chinese albert_base_chinese_ner_pipeline pipeline BertForTokenClassification from ckiplab
author: John Snow Labs
name: albert_base_chinese_ner_pipeline
date: 2024-09-01
tags: [zh, open_source, pipeline, onnx]
task: Named Entity Recognition
language: zh
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`albert_base_chinese_ner_pipeline` is a Chinese model originally trained by ckiplab.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/albert_base_chinese_ner_pipeline_zh_5.4.2_3.0_1725163438136.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/albert_base_chinese_ner_pipeline_zh_5.4.2_3.0_1725163438136.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("albert_base_chinese_ner_pipeline", lang = "zh")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("albert_base_chinese_ner_pipeline", lang = "zh")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|albert_base_chinese_ner_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|zh|
|Size:|37.8 MB|

## References

https://huggingface.co/ckiplab/albert-base-chinese-ner

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForTokenClassification