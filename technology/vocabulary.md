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

<table><thead><tr><th width="134.85546875">Code</th><th width="142.5625">Structural Role</th><th>Description</th></tr></thead><tbody><tr><td>Generation</td><td>Primary authorship</td><td>AI produces the primary or full content. Human involvement is limited to prompting, selection, curation, or review.</td></tr><tr><td>Co-Creation</td><td>Shared authorship</td><td>AI and human jointly produce the content through an interdependent process. AI generates substantial, integrated parts based on human-created material, structure, or constraints, and the resulting authorship is not cleanly separable.</td></tr><tr><td>Contribution</td><td>Partial creative input</td><td>AI produces discrete content elements such as fragments, ideas, or corrections that a human selectively integrates into a human-authored work. The human remains editor and final author.</td></tr><tr><td>Enhancement</td><td>Structural or content extension</td><td>AI modifies or extends existing content to improve quality, richness, or structure. Changes may be substantial but do not replace original authorship.</td></tr><tr><td>Refinement</td><td>Polishing / minor adjustments</td><td>AI performs limited, surface-level adjustments that preserve the existing structure, meaning, and authorship.</td></tr><tr><td>Transformation</td><td>Re-expression</td><td>AI converts existing content into another form while preserving semantic equivalence or an explicit link to the original.</td></tr><tr><td>Analysis</td><td>Interpretation / extraction</td><td>AI interprets existing content to derive structure, features, metadata, meaning, or insights, without producing new expressive content.</td></tr></tbody></table>

Structural role indicates the degree and nature of AI involvement in the creation or modification of the final content, assessed from the perspective of the content itself.

These codes allow content operations to be described consistently across different media sectors and types.

## System Attribution (How It Was Done)

Transparency about AI involvement can include providing details about which specific systems were used, though these details are optional. FAIA uses two key attribution fields:

**Provider**

Definition: The company, organization, or entity that publishes or operates the AI tool or model. This identifies who is responsible for developing, training, and deploying the AI system.

Examples: `OpenAI, Anthropic, Stability AI, Adobe, ElevenLabs, Meta, Google DeepMind`

**Model**

Definition: The specific AI model or family of models that generated or modified the content. This goes beyond the provider to identify the particular system version or architecture used.

Examples: `GPT-4o, Claude-3.5-Sonnet, Stable-Diffusion-v3, Whisper-large-v3, Sora-1.0, DALL-E-3, Llama-3.1-405B`

<br>
