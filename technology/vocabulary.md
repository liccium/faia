# Vocabulary

The FAIA Vocabulary is designed to **transparently and consistently disclose the role of AI in the content creation process**. It provides a standardised way to describe how content is created, modified, or generated in workflows involving both human and AI contributions.

Rather than defining a new set of terms, the vocabulary aligns with existing domain-specific standards where applicable and fills gaps with media-independent codes. It supports machine-readable declarations and integrates with provenance, attribution, and rights metadata systems.

<figure><img src="../.gitbook/assets/Layer.png" alt=""><figcaption></figcaption></figure>

## FAIA Flags (AI Involvement)

**FAIA Flags** provide high-level signals of AI involvement. These flags can be applied across media types – including text, images, audio, and video – and assigned at the asset or record level.

<table><thead><tr><th width="78.13671875" align="center">Flag</th><th width="105.33203125">Name</th><th>Description</th></tr></thead><tbody><tr><td align="center">HCC</td><td>Human-Created Content</td><td>Content created, generated and edited exclusively by humans or human-controlled instruments. While digital tools such as word processors, image editors, or audio software may be used, no generative AI systems are involved at any stage of the creative or editorial process.</td></tr><tr><td align="center">AAC</td><td>AI-Assisted Content</td><td>Content where a human or a human-controlled instrument remains the primary creator and AI systems contributed during the creation process to various degrees. This may include AI-generated input that humans or human-controlled instruments accept or reject, generation of content fragments that humans or human-controlled instruments integrate into larger works, or refinement steps performed under direct human supervision and editorial control.</td></tr><tr><td align="center">AIG</td><td>AI-Generated Content</td><td>Content generated predominantly or entirely by an AI system, where the AI serves as the main creative agent. Human input is limited to initiating prompts, selecting among AI-generated outputs, or making minor adjustments that do not materially alter structure, substance, or expressive intent. The resulting content is accepted largely as produced by the AI, with no substantive human editing or creatorship.</td></tr></tbody></table>

## Activity Types

**Activity Types** describe, with more granularity, what was done to the content during creation or editing. Activity Types indicate specific operations such as editing, summarisation, transformation, translation, or full generation.

FAIA supports the use of established vocabularies:

* **STM AI Classification**\
  Developed by the STM Association, this framework identifies how AI tools are used during preparation of academic manuscripts – including classification, translation, summarisation, or visualisation. \
  [See STM report](https://stm-assoc.org/new-stm-draft-report-classifying-ai-use-in-manuscript-preparation/)

Where such domain-specific vocabularies are not applicable, the FAIA project defines a set of **generic, media-independent activity types**, such as:

<table><thead><tr><th width="134.85546875">Code</th><th width="142.5625">Structural Role</th><th>Description</th></tr></thead><tbody><tr><td>Co-Creation</td><td>Shared authorship</td><td>AI and humans jointly produce content through an interactive process. The AI generates substantial parts of the content based directly on human-created material and structure. Creatorship is shared and not clearly separable.</td></tr><tr><td>Contribution</td><td>Partial creative input</td><td>AI produces content that is incorporated into a primarily human-created work. The human determines overall structure, intent, and final form, and remains the final creator of the combined result.</td></tr><tr><td>Enhancement</td><td>Structural or content extension</td><td>AI modifies or extends existing human-created content to improve quality, clarity, richness, or structure.</td></tr><tr><td>Refinement</td><td>Polishing / minor adjustments</td><td>AI performs limited adjustments that preserve the existing structure, meaning, and creatorship of the content.</td></tr><tr><td>Transformation</td><td>Re-expression</td><td>AI converts existing content into another form or representation while preserving semantic equivalence or maintaining a close relationship to the original content.</td></tr><tr><td>Analysis</td><td>Interpretation / extraction</td><td>AI interprets existing content to derive structure, features, metadata, meaning, or insights.</td></tr></tbody></table>

Structural role indicates the degree and nature of AI involvement in the creation or modification of the final content, assessed from the perspective of the content itself.

These codes allow content operations to be described consistently across different media sectors and types.

## System Attribution

Transparency about AI involvement can include providing details about which specific systems were used, though these details are optional. FAIA uses two key attribution fields:

**Provider**

Definition: The company, organization, or entity that publishes or operates the AI tool or model. This identifies who is responsible for developing, training, and deploying the AI system.

Examples: `OpenAI, Anthropic, Stability AI, Adobe, ElevenLabs, Meta, Google DeepMind`

**Model**

Definition: The specific AI model or family of models that generated or modified the content. This goes beyond the provider to identify the particular system version or architecture used.

Examples: `GPT-4o, Claude-3.5-Sonnet, Stable-Diffusion-v3, Whisper-large-v3, Sora-1.0, DALL-E-3, Llama-3.1-405B`

<br>
