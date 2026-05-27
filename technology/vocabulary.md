---
layout:
  width: default
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
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
---

# Vocabulary

The FAIA Vocabulary defines structured and machine-readable terms for describing AI involvement in the creation, modification, and processing of digital content.

The framework distinguishes between:

* **high-level attribution categories** describing the relationship between human and AI contribution
* **activity codes** describing how AI systems were used during content workflows
* **system attribution** identifying the AI system and version involved

The vocabulary is designed to support interoperable AI attribution across different media types, workflows, publishing environments, platforms, and technical systems.

FAIA semantic resources are published as open vocabularies and ontologies using persistent identifiers and semantic web standards including JSON-LD and RDF.

<figure><img src="../.gitbook/assets/FAIA Model_new_new.png" alt=""><figcaption></figcaption></figure>

## FAIA Flags

FAIA Flags classify the overall relationship between human and AI contribution within the resulting content asset.

The flags are media-independent and may be applied to text, images, audio, video, datasets, software, or mixed-media workflows.

The flags describe the degree of human authorship and responsibility rather than the specific technical operation performed by the AI system.

<div align="left"><figure><img src="../.gitbook/assets/Property 1=HCC.svg" alt=""><figcaption></figcaption></figure></div>

**Human-Created Content**

Content created, generated and edited exclusively by humans or human-controlled instruments. While digital tools such as word processors, image editors, or audio software may be used, no generative AI systems are involved at any stage of the creative or editorial process.

<div align="left"><figure><img src="../.gitbook/assets/Property 1=AAC.svg" alt=""><figcaption></figcaption></figure></div>

**AI-Assisted Content**

Content where a human or a human-controlled instrument remains the primary creator and AI systems contributed during the creation process to various degrees. This may include AI-generated input that humans or human-controlled instruments accept or reject, generation of content fragments that humans or human-controlled instruments integrate into larger works, or refinement steps performed under direct human supervision and editorial control.

<div align="left"><figure><img src="../.gitbook/assets/Property 1=AIG.svg" alt=""><figcaption></figcaption></figure></div>

**AI-Generated Content**

Content generated predominantly or entirely by an AI system, where the AI serves as the main creative agent. Human input is limited to initiating prompts, selecting among AI-generated outputs, or making minor adjustments that do not materially alter structure, substance, or expressive intent. The resulting content is accepted largely as produced by the AI, with no substantive human editing or creatorship.

## Activity Codes

Activity Codes describe how AI systems were used during the content lifecycle. While the FAIA Flags classify the overall nature of the resulting content, Activity Types describe the structural role AI played within the workflow.



<table><thead><tr><th width="140.984375">Code</th><th width="189.19140625">What the human provides</th><th width="293.98046875">What the AI provides</th></tr></thead><tbody><tr><td><strong>Co-Creation</strong></td><td>Core ideas, structure, or source material</td><td>Independent sections, elements, or content developed jointly</td></tr><tr><td><strong>Contribution</strong></td><td>Overall structure and intent</td><td>Discrete components integrated by the human</td></tr><tr><td><strong>Enhancement</strong></td><td>Existing content</td><td>Extensions or quality improvements</td></tr><tr><td><strong>Refinement</strong></td><td>Existing content</td><td>Minor surface-level or technical adjustments</td></tr><tr><td><strong>Transformation</strong></td><td>Prompt or task definition</td><td>Autonomous re-expression into another form</td></tr><tr><td><strong>Analysis</strong></td><td>Prompt or analytical instruction</td><td>Automated extraction, classification, or metadata generation</td></tr></tbody></table>

FAIA is designed to complement existing sector-specific standards and metadata ecosystems where appropriate. Examples include:

* **STM AI Classification**\
  Developed by the STM Association, this framework identifies how AI tools are used during preparation of academic manuscripts – including classification, translation, summarisation, or visualisation. [See STM report](https://stm-assoc.org/new-stm-draft-report-classifying-ai-use-in-manuscript-preparation/)
* IPTC Digital Source Types for photography and news media&#x20;

## System Attribution

Transparency about AI involvement often requires more than simply stating that AI was used. In many workflows it is also important to identify which AI system contributed to the content and which version of that system was used at the time of creation or modification.

Different systems and model versions may differ substantially in behaviour, capabilities, limitations, training data composition, and licensing conditions.

FAIA supports two structured attribution fields:

**System**

The AI system or engine used to generate or modify the content. This identifies the technical system responsible for producing the output, using its official designation.

Examples: `ChatGPT, DALL-E, Google Gemini, Claude`

**Version**

Definition: The specific release or version of the AI system used. This follows the naming or numbering scheme defined by the system’s operator, where available.

Examples: `GPT-5.2, Claude Opus 4.6`

### Machine-Readable and Interoperable

The FAIA Vocabulary is designed for machine-readable implementation using semantic web standards including JSON-LD, RDF vocabularies, and interoperable metadata schemas.

The framework follows FAIR principles – Findability, Accessibility, Interoperability, and Reusability – and was developed in collaboration with the GO FAIR Foundation to support open, interoperable, and reusable attribution infrastructure across different technical and institutional environments.

The vocabulary and ontology are published through persistent identifiers and may be integrated into APIs, registries, publishing systems, provenance frameworks, and verification services.

Semantic resources:

* [https://w3id.org/liccium/faia/ont/0.4.0.ttl](https://w3id.org/liccium/faia/ont/0.4.0.ttl)
* [https://w3id.org/liccium/faia/vocab/0.4.0.ttl](https://w3id.org/liccium/faia/vocab/0.4.0.ttl)

The framework is implementation-independent and intended to support interoperable adoption across different applications, platforms, registries, and service providers.

<br>
