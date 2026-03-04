# CLAUDE.md - Engineering Guidelines for PADI Ontologies

## Technical Vision
This repository maintains the formal logic for the **Practice-Area Depth Index (PADI)**. All contributions must align with **Library Science classification principles** and **OWL 2 DL** standards.

## Coding Standards (RDF/Turtle)
- **Format**: Always use Turtle (`.ttl`) for human-machine readability.
- **Naming**: Use PascalCase for Classes (e.g., `padi:CaseSubtype`) and camelCase for Properties (e.g., `padi:hasDepthScore`).
- **Metadata**: Every new class MUST have an `rdfs:label` and `rdfs:comment` to ensure semantic clarity.

## Logic Enforcement
- **Cardinality**: Ensure all SHACL shapes enforce the PADI-standard $\ge 3$ subtype rule.
- **Validation**: Before committing, verify the ontology against the `padi-validation.ttl` shapes.

## Scholarly Tone
When assisting with code documentation, use precise **Information Science** terminology. Refer to the hierarchy as a **Knowledge Organization System (KOS)**, not a "category list."
