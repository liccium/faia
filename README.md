# FAIR AI Attribution (FAIA)

## The FAIA Project

**FAIA – FAIR AI Attribution** – is an open framework for structured, machine-readable, and verifiable disclosure of AI involvement in digital content creation. The project is developed by [**Liccium**](https://liccium.com/) in collaboration with [**Leiden University**](https://www.universiteitleiden.nl/en) and the [**GO FAIR Foundation**](https://www.gofair.foundation/) in response to the growing need for transparency, provenance, and accountability in digital publishing, research communication, and media production.

As generative AI systems become increasingly integrated into writing, editing, design, publishing, and content production workflows, it is becoming progressively more difficult to distinguish between human-created, AI-assisted, and AI-generated material. At the same time, existing disclosure approaches are fragmented, inconsistent, and often technically fragile. Metadata may be removed during distribution, platform-specific labels rarely persist across environments, and there is currently no widely adopted infrastructure for interoperable and verifiable AI attribution.

FAIA addresses this problem by providing a shared attribution vocabulary together with technical mechanisms for persistent and verifiable declarations. The framework enables creators, publishers, researchers, platforms, and AI providers to disclose whether and how AI systems contributed to the creation or modification of digital content.

<figure><img src=".gitbook/assets/FAIA Explorer@2x.png" alt=""><figcaption><p>FAIA Registry Explorer, <a href="https://faia.io/">https://faia.io</a></p></figcaption></figure>

## **Why is FAIA necessary?**

The rapid growth of AI-generated content creates significant challenges for digital ecosystems:

* **reduced trust** in digital information and media authenticity
* difficulties in documenting **editorial and research integrity**
* increasing **regulatory transparency requirements**
* challenges for **provenance verification** and reproducibility
* contamination risks for future AI training datasets

These challenges are increasingly recognised in policy and regulatory frameworks, including the European Union AI Act, which introduces transparency obligations for AI-generated and AI-manipulated content.

FAIA contributes to addressing these challenges by enabling AI involvement to be disclosed in a way that is:

* **machine-readable**
* **interoperable** across systems and platforms
* **cryptographically verifiable**
* **persistently linked** to digital content
* resolvable independently of individual platforms or publication environments

## Goals and Scope

The FAIA framework provides a practical and implementation-independent foundation for AI attribution across digital media ecosystems. The framework is designed to work across text, images, audio, video, datasets, and mixed-media workflows.

Its core goals are to:

* enable **transparent disclosure** **of AI involvement** in content creation and modification
* support **interoperable attribution** across platforms, workflows, and media types
* strengthen **provenance, accountability, and trust** in digital publishing and research environments
* **support emerging transparency and compliance requirements**
* provide infrastructure for downstream services such as verification, moderation, dataset filtering, and provenance analysis

## Technical Foundation

FAIA combines semantic metadata, persistent identifiers, digital signatures, and interoperable registry infrastructure to support durable AI attribution workflows.

Within the reference implementation developed in the FAIA project ecosystem:

* **FAIR AI attribution metadata** is expressed in machine-readable form using semantic web standards
* declarations are **persistently linked to content through ISCC fingerprints**
* declarations may be **digitally signed** using certificates or verifiable credentials
* declaration records may be published and resolved through **interoperable registry infrastructure**
* APIs and semantic vocabularies **support integration** into external applications and publishing workflows

The framework is implementation-independent and does not depend on a single platform, registry operator, or software vendor. Third parties are encouraged to integrate FAIA-compatible workflows and services using the published vocabularies, APIs, and interoperability mechanisms.

## Current Implementations

Current prototype implementations developed within the FAIA project ecosystem include:

* the FAIA **Statement Generator:** \
  [https://www.faia.io/statement-generator](https://www.faia.io/statement-generator)
* **machine-readable attribution vocabularies and ontologies**:\
  [https://github.com/liccium/w3id.docs](https://github.com/liccium/w3id.docs)&#x20;
* openly documented **declaration APIs**\
  [https://dev.liccium.com](https://dev.liccium.com/)
* **registry explorer** infrastructure\
  [https://faia.io](https://faia.io/)
* **trust infrastructure** based on digital signatures and verifiable credentials\
  [https://creatorcredentials.com](https://creatorcredentials.com/)

Work is also ongoing on user-facing applications and federated registry infrastructure supporting broader ecosystem participation and interoperable deployment across independent platforms and services.

## Outcomes and Impact

FAIA aims to support more transparent and accountable digital publishing and AI ecosystems by:

* enabling **creators and organisations to disclose AI involvement** consistently and verifiably
* supporting **provenance and integrity workflows** across publishing and research environments
* helping platforms and downstream services **interpret attribution metadata programmatically**
* supporting **future verification, moderation, and dataset management** workflows
* reducing fragmentation across AI transparency approaches and metadata systems

While the framework is intended as a cross-sector infrastructure applicable to all forms of digital media, early implementations and collaborations have focused particularly on academic publishing, research communication, and professional publishing environments.

FAIA contributes to the development of open and interoperable infrastructure for AI attribution that remains portable across platforms, resilient across distribution environments, and accessible across different technical and institutional ecosystems.
