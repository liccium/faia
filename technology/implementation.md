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

# Reference Implementations

FAIA supports different levels of implementation depending on the required level of persistence, verification, and infrastructure integration.

## FAIA Statement Generator

The FAIA Statement Generator provides a lightweight mechanism for creating portable AI attribution statements using the FAIA vocabulary.

[https://www.faia.io/statement-generator](https://www.faia.io/statement-generator)

The generated statements can be embedded into websites, attached to publications, or shared alongside digital content. They support both human-readable and machine-readable disclosure of AI involvement.

However, these statements are not persistently bound to the content and are not independently verifiable. Without cryptographic signing, registry publication, and persistent content–metadata binding, there is no reliable mechanism to verify authorship, integrity, or long-term association with the underlying asset.

<figure><img src="../.gitbook/assets/CleanShot 2026-05-27 at 20.36.36@2x.png" alt=""><figcaption></figcaption></figure>

## Liccium Reference Implementation

The Liccium platform provides a reference implementation of persistent and verifiable FAIA declarations.

The implementation combines:

* ISCC-based content fingerprinting
* machine-readable JSON-LD declaration metadata
* cryptographic signatures and verifiable credentials
* declaration APIs
* federated registry infrastructure

Using the Liccium implementation, FAIA declarations can be:

* created through applications or APIs
* digitally signed by the declarant
* persistently linked to digital content through ISCC identifiers
* published to interoperable registry infrastructure
* independently resolved and verified across platforms and workflows

The implementation includes the Liccium Declaration API, registry infrastructure, and user-facing applications supporting declaration creation, signing, publication, and verification workflows.
