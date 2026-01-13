# Vocabulary

The FAIA Vocabulary is designed to **transparently and consistently disclose the role of AI in the content creation process**. It provides a standardised way to describe how content is created, modified, or generated in workflows involving both human and AI contributions.

Rather than defining a new set of terms, the vocabulary aligns with existing domain-specific standards where applicable and fills gaps with media-independent codes. It supports machine-readable declarations and integrates with provenance, attribution, and rights metadata systems.

<figure><img src="../.gitbook/assets/FAIA Framework.jpg" alt=""><figcaption></figcaption></figure>

## FAIA Flags (AI Involvement)

**FAIA Flags** provide high-level signals of AI involvement. These flags can be applied across media types – including text, images, audio, and video – and assigned at the asset or record level.

<table><thead><tr><th width="78.13671875" align="center">Flag</th><th width="105.33203125">Name</th><th>Description</th></tr></thead><tbody><tr><td align="center">HCC</td><td>Human-Created Content</td><td>Content created and edited exclusively by humans. While digital tools may be used, no AI systems are involved at any stage of the creative or editorial process.</td></tr><tr><td align="center">AAC</td><td>AI-Assisted Content</td><td>Content where a human remains the primary author but AI systems contributed during the process. This may include suggestions, generation of fragments, or refinement steps performed under human supervision and editorial control.</td></tr><tr><td align="center">AIG</td><td>AI-Generated Content</td><td>Content generated predominantly or entirely by an AI system. The AI is the main creative agent. Human input may be limited to initiating a prompt or selecting from outputs, with minimal or no human editing or authorship applied.</td></tr></tbody></table>

## Activity Types (What Was Done)

**Activity Types** describe, with more granularity, what was done to the content during creation or editing. Activity Types indicate specific operations such as editing, summarisation, transformation, translation, or full generation.

FAIA supports the use of established vocabularies:

* **IPTC Digital Source Type**\
  Widely adopted in the news and media industries and professional photography, IPTC provides a framework to describe origin and provenance of visual content, indicating whether it was captured directly, digitised, created or modified by software.\
  [See IPTC guidance](https://www.iptc.org/std/photometadata/documentation/userguide/#_guidance_for_using_digital_source_type)
* **STM AI Classification**\
  Developed by the STM Association, this framework identifies how AI tools are used during preparation of academic manuscripts – including classification, translation, summarisation, or visualisation. \
  [See STM report](https://stm-assoc.org/new-stm-draft-report-classifying-ai-use-in-manuscript-preparation/)

Where such domain-specific vocabularies are not applicable, the FAIA project defines a set of **generic, media-independent activity types**, such as:

<table><thead><tr><th width="134.85546875">Code</th><th width="142.5625">Structural Role</th><th>Description</th></tr></thead><tbody><tr><td>Generation</td><td>Primary creation</td><td>AI produces the primary or full content; human role limited to prompting, curation, or review.</td></tr><tr><td>Co-Creation</td><td></td><td>AI generates substantial, integrated parts of the content based directly on human-created material, structure, or constraints; authorship is shared and not cleanly separable.</td></tr><tr><td>Contribution</td><td>Partial creative input</td><td>AI produces discrete content elements (fragments, ideas, or corrections) that a human selectively integrates into a human-authored work; the human remains editor and final author.</td></tr><tr><td>Enhancement</td><td>Structural / content extension</td><td>AI modifies or extends content to improve quality, presentation, or structure. Can involve substantial changes or additions.<br>AI modifies, augments or extends existing content to improve quality, richness, or structure. Can involve substantial changes or additions, without replacing original authorship.</td></tr><tr><td>Refinement</td><td>Polishing / minor adjustments</td><td>AI performs limited, surface-level adjustments that preserve existing structure, meaning, and authorship.</td></tr><tr><td>Transformation</td><td>Re-expression</td><td>AI transforms or converts existing content into another form while retaining semantic equivalence or link.</td></tr><tr><td>Analysis</td><td>Interpretation / extraction</td><td>AI interprets existing content to extract structure, features, metadata, meaning, or insights from it.</td></tr></tbody></table>

These codes allow content operations to be described consistently across different media sectors and types.

## System Attribution (How It Was Done)

If the actor is an AI system, FAIA includes a set of metadata fields to describe the system used:

* **Tool** – Name of the interface or product (e.g. `"ChatGPT"`).
* **Model** – Underlying model used (e.g. `"GPT-4o"`).
* **Version** – Version number of the tool or model (e.g. `"4.0"`).
* **Provider** – Entity providing the system (e.g. `"OpenAI"`).
