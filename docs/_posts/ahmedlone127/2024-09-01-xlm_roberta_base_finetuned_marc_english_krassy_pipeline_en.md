---
layout: model
title: English xlm_roberta_base_finetuned_marc_english_krassy_pipeline pipeline XlmRoBertaForSequenceClassification from Krassy
author: John Snow Labs
name: xlm_roberta_base_finetuned_marc_english_krassy_pipeline
date: 2024-09-01
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

Pretrained XlmRoBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`xlm_roberta_base_finetuned_marc_english_krassy_pipeline` is a English model originally trained by Krassy.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/xlm_roberta_base_finetuned_marc_english_krassy_pipeline_en_5.4.2_3.0_1725189959679.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/xlm_roberta_base_finetuned_marc_english_krassy_pipeline_en_5.4.2_3.0_1725189959679.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("xlm_roberta_base_finetuned_marc_english_krassy_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("xlm_roberta_base_finetuned_marc_english_krassy_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|xlm_roberta_base_finetuned_marc_english_krassy_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|833.5 MB|

## References

https://huggingface.co/Krassy/xlm-roberta-base-finetuned-marc-en

## Included Models

- DocumentAssembler
- TokenizerModel
- XlmRoBertaForSequenceClassification