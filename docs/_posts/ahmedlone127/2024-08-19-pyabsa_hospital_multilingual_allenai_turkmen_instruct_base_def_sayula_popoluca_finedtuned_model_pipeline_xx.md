---
layout: model
title: Multilingual pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline pipeline T5Transformer from amir22010
author: John Snow Labs
name: pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline
date: 2024-08-19
tags: [xx, open_source, pipeline, onnx]
task: [Question Answering, Summarization, Translation, Text Generation]
language: xx
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained T5Transformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline` is a Multilingual model originally trained by amir22010.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline_xx_5.4.2_3.0_1724053466432.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline_xx_5.4.2_3.0_1724053466432.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline", lang = "xx")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline", lang = "xx")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|pyabsa_hospital_multilingual_allenai_turkmen_instruct_base_def_sayula_popoluca_finedtuned_model_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|xx|
|Size:|936.9 MB|

## References

https://huggingface.co/amir22010/PyABSA_Hospital_Multilingual_allenai_tk-instruct-base-def-pos_FinedTuned_Model

## Included Models

- DocumentAssembler
- T5Transformer