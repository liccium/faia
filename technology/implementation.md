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

# Implementation

## The Liccium Platform

The FAIA attribution framework is integrated into the [**Liccium platform**](https://liccium.com/) as a plugin. This enables creators, researchers, publishers, and platforms to declare AI involvement directly within their content authentication workflows. Designed to be intuitive yet technically robust, the plugin supports transparency, compliance, and interoperability by making AI contributions to content creation verifiable and persistently linked to the original work.

<figure><img src="../.gitbook/assets/Screen.png" alt=""><figcaption><p>Liccium application</p></figcaption></figure>

## How does it work?

### **1. Select the Type of AI Involvement**

Users can choose from a set of standardised **Attribution Flags** that reflect the degree and nature of AI’s contribution. These include categories such as:

<table><thead><tr><th width="87.62890625" align="center">Flage Code</th><th width="196.65625">Name</th><th>Description</th></tr></thead><tbody><tr><td align="center">HCC</td><td>Human-Created Content</td><td>Content created and edited entirely by humans. May involve digital tools, but no AI involvement at any stage.</td></tr><tr><td align="center">AAE</td><td>AI-Assisted Editing</td><td>AI is used only after initial creation—for grammar, formatting, cleanup, upscaling, or similar editorial improvements. No AI-generated content added.</td></tr><tr><td align="center">AAC</td><td>AI-Assisted Contribution</td><td>AI contributes during the creation process, such as suggesting content, generating fragments, or shaping drafts, under human direction and control.</td></tr><tr><td align="center">ACO</td><td>AI–Human Co-Creation</td><td>AI and human share creative responsibility. Content results from iterative collaboration or joint authorship between human and AI.</td></tr><tr><td align="center">AGC</td><td>AI-Generated Content</td><td>AI is the primary creator. Human input is limited to initiating or curating. Little to no human editing or creative direction is applied post-output.</td></tr></tbody></table>

This classification ensures consistent disclosure across diverse media formats and sectors.

_<mark style="color:red;">Be aware that the framework is still in development!</mark>_&#x20;

### **2. Provide Contextual Metadata**

Beyond the basic attribution flag, users may optionally provide additional details that clarify how AI was involved, including:

* The name and version of the AI tool (e.g. _ChatGPT-4_, _Midjourney v6_)
* The specific function it served (e.g. _summarisation_, _translation_, _image enhancement_)
* Workflow context or editorial stage (e.g. _used in initial drafting_, _applied during peer review_)

These metadata elements improve transparency and support reuse, audit, and regulatory evaluation.

_<mark style="color:red;">Be aware that the framework is still in development!</mark>_&#x20;

### **3. Bind to the ISCC Code**

All FAIA declarations are **cryptographically bound** to the **International Standard Content Code (ISCC)**, a content-derived identifier and ISO standard (ISO 24138). This ensures that attribution metadata remains uniquely and persistently associated with the content – even if the asset is modified and redistributed.

### **4. Generate Verifiable, Timestamped Declarations**

Every declaration is digitally signed using  **Verifiable Credential (VC)** or **DID keys** of the creator. The declaration is stored as a tamper-evident **JSON-LD file (nanopublication)**, including a trusted timestamp. This guarantees the authenticity and integrity of the AI attribution data.

### **5. Register in the Liccium Registry**

The declarations are published to a **public, decentralised registry** operated by Liccium, making them:

* **Publicly resolvable** using content identifiers like the ISCC
* **Searchable** for researchers, platforms, and compliance tools
* **Auditable** under regulatory regimes such as the EU AI Act (e.g. Article 50 disclosure obligations)

This registry ensures lasting transparency and verifiability in content attribution and provenance.
