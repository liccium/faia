---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Vocabulary

## Attribution Flags

At the heart of the FAIA framework is a controlled vocabulary designed to transparently and consistently disclose the role of AI in the content creation process. This vocabulary introduces standardised **Attribution Flags** that classify content based on how and to what extent AI was involved.&#x20;

<figure><img src="../.gitbook/assets/FAIA-Slide.jpg" alt="" width="563"><figcaption><p>(Draft) </p></figcaption></figure>

These flags include categories such as (_work in progress_):

* **Human-Created Content (HCC)**
* **AI-Assisted Content (AAC)**
* **AI-Generated Content (AIG)**
* **Human-Edited AI Content (HEAIG)**
* **AI-Supported Editorial Processes (AISEP)**

This general-purpose taxonomy applies across media types – text, images, audio, and video – and forms the foundation for verifiable content declarations in the Liccium ecosystem.

## **Alignment with Existing Standards and Frameworks**

FAIA builds upon and complements existing classification efforts:

* The vocabulary draws conceptual inspiration from the **IPTC Digital Source Type**, widely used in photo metadata, which introduces high-level source categories for digital content. FAIA generalizes this approach and applies it uniformly across media formats and publishing contexts.\
  [See IPTC guidance](https://www.iptc.org/std/photometadata/documentation/userguide/#_guidance_for_using_digital_source_type)
* FAIA is also designed to integrate with more domain-specific frameworks like the **STM Association’s AI Classification for Manuscript Preparation**, which focuses on the concrete ways AI tools are used during the research and editorial process (e.g., summarisation, translation, visualisation).\
  [See STM report](https://stm-assoc.org/new-stm-draft-report-classifying-ai-use-in-manuscript-preparation/)

While STM’s system zooms in on **how** AI was used, FAIA answers a broader question: **what** is the content, in terms of origin and AI involvement. FAIA and STM can be layered together – for example, a document declared as _AI-Assisted Content (AAC)_ under FAIA may include STM-style annotations such as “AI-supported data visualization” or “AI-assisted translation.”

## **Future Interoperability**

FAIA recommends a modular approach where detailed activity labels from sector-specific frameworks are embedded within broader content-level declarations. This enables:

* Machine-readable metadata with consistent flags across sectors
* Compatibility with editorial systems, registries, and compliance tools
* Support for persistent, signed provenance records using technologies like Verifiable Credentials and ISCC

By integrating fine-grained classifications into FAIA’s general-purpose framework, content declarations can serve a wide range of stakeholders – from researchers and publishers to regulators and AI model developers – ensuring that AI attribution is both **transparent and technically actionable**.
