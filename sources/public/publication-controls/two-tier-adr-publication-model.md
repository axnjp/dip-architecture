# Two-Tier ADR Publication Model

Status: `approved and active`  
Classification: Public Reference Architecture  
Approved in: `P0-B27`

## Purpose

The ADR corpus uses two coordinated publication forms so public architectural accountability does not disclose protected topology, restricted evidence, or the existence of any real protected instance.

## Public ADR projection

Every public ADR projection preserves:

- the existing ADR identifier and approved title;
- accepted and locked lifecycle status;
- an abstract public decision statement;
- public consequences and conformance obligations;
- an explicit disclosure-boundary statement.

It excludes:

- approval-message quotations and message locators;
- restricted source identifiers and evidence-package locations;
- protected authority roots, provider details, configuration paths, and secret-resolution topology;
- real instance identifiers, memberships, bindings, or active private configuration;
- language implying that any real protected instance exists.

## Restricted ADR body

The separately authenticated architecture-evidence repository retains the complete normalized ADR body, detailed topology, source and approval evidence, and verification relationships. It remains subject to the prohibition on Private Authority data and secret values.

## Authority relationship

The two forms share one ADR identifier and one accepted decision. The public projection is not a competing decision, redaction of a loaded restricted build input, or a replacement for the complete body. It is a deterministic public derivative produced from an explicit allowlist and disclosure policy.

## Release rule

No public ADR projection may enter a release until it passes semantic disclosure review. Release evidence must prove that the public build used only public projections and never loaded the restricted ADR corpus.
