---
layout: model
title: Danish xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline pipeline XlmRoBertaForQuestionAnswering from saattrupdan
author: John Snow Labs
name: xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline
date: 2024-09-01
tags: [da, open_source, pipeline, onnx]
task: Question Answering
language: da
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained XlmRoBertaForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline` is a Danish model originally trained by saattrupdan.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline_da_5.4.2_3.0_1725156320182.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline_da_5.4.2_3.0_1725156320182.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline", lang = "da")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline", lang = "da")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|xlm_roberta_qa_xlmr_base_texas_squad_danish_danish_saattrupdan_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|da|
|Size:|877.6 MB|

## References

https://huggingface.co/saattrupdan/xlmr-base-texas-squad-da

## Included Models

- MultiDocumentAssembler
- XlmRoBertaForQuestionAnswering