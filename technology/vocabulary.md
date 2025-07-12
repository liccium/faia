# Vocabulary

## Attribution Flags

The FAIA Vocabulary is designed to **transparently and consistently disclose the role of AI in the content creation process**. It provides a standardised way to describe how content is created, modified, or generated in workflows involving both human and AI contributions.

Rather than defining a new set of terms, the vocabulary aligns with existing domain-specific standards where applicable and fills gaps with media-independent codes. It supports machine-readable declarations and integrates with provenance, attribution, and rights metadata systems.

<figure><img src="../.gitbook/assets/FAIA Model (1).png" alt=""><figcaption></figcaption></figure>

## FAIA Flags (AI Involvement)

**FAIA Flags** classify the overall content at the top level, giving a quick indication of the degree of AI involvement:

* **Human-Created Content (HCC)** – content produced without AI involvement.
* **AI-Assisted Content (AAC)** – content where AI systems contributed to or modified human input.
* **AI-Generated Content (AIG)** – content generated entirely or predominantly by AI systems.

These flags apply across media types – including text, images, audio, and video – and can be assigned at the asset or record level.

## Activity Types (What Was Done)

**Activity Types** describe, with more granularity, what was done to the content. They indicate specific operations such as editing, summarisation, transformation, or full generation.

FAIA supports the use of established vocabularies:

* **IPTC Digital Source Type**\
  Widely adopted in photo metadata, this vocabulary distinguishes between original, edited, and AI-generated visual content.\
  [See IPTC guidance](https://www.iptc.org/std/photometadata/documentation/userguide/#_guidance_for_using_digital_source_type)
* **STM AI Classification**\
  Developed by the STM Association, this schema identifies how AI tools are used during manuscript preparation – including classification, translation, summarisation, or visualisation.\
  [See STM report](https://stm-assoc.org/new-stm-draft-report-classifying-ai-use-in-manuscript-preparation/)

Where such domain-specific vocabularies are not applicable, FAIA defines a set of **generic, media-independent activity types**, including:

* `Capture`
* `Contribution`
* `Transformation`
* `Enhancement`
* `Generation`

These codes allow content operations to be described consistently across different sectors and tools.

## Actor (Who Did It)

The **Actor** is the entity responsible for performing a declared activity. Each activity can be attributed to a an actor:

* `Human Actor` – A person performed the activity.
* `AI Actor` – An automated system performed the activity.

This distinction clarifies authorship and responsibility and is essential for downstream use in rights, attribution, or provenance frameworks.

## System Attribution (How It Was Done)

If the actor is an AI system, FAIA includes a set of metadata fields to describe the system used:

* **Tool** – Name of the interface or product (e.g. `"ChatGPT"`).
* **Model** – Underlying model used (e.g. `"GPT-4o"`).
* **Version** – Version number of the tool or model (e.g. `"4.0"`).
* **Provider** – Entity providing the system (e.g. `"OpenAI"`).
