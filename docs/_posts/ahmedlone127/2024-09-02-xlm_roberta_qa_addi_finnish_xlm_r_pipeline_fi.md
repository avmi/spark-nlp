---
layout: model
title: Finnish xlm_roberta_qa_addi_finnish_xlm_r_pipeline pipeline XlmRoBertaForQuestionAnswering from Gantenbein
author: John Snow Labs
name: xlm_roberta_qa_addi_finnish_xlm_r_pipeline
date: 2024-09-02
tags: [fi, open_source, pipeline, onnx]
task: Question Answering
language: fi
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained XlmRoBertaForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`xlm_roberta_qa_addi_finnish_xlm_r_pipeline` is a Finnish model originally trained by Gantenbein.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/xlm_roberta_qa_addi_finnish_xlm_r_pipeline_fi_5.5.0_3.0_1725236347329.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/xlm_roberta_qa_addi_finnish_xlm_r_pipeline_fi_5.5.0_3.0_1725236347329.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("xlm_roberta_qa_addi_finnish_xlm_r_pipeline", lang = "fi")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("xlm_roberta_qa_addi_finnish_xlm_r_pipeline", lang = "fi")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|xlm_roberta_qa_addi_finnish_xlm_r_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|fi|
|Size:|777.3 MB|

## References

https://huggingface.co/Gantenbein/ADDI-FI-XLM-R

## Included Models

- MultiDocumentAssembler
- XlmRoBertaForQuestionAnswering