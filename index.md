# PADI Technical Whitepaper: The v2.0 Specification
**Founding Architect:** Samuel Muriithi | *The Peculiar Librarian*

## 1. The 1003 Cardinality Rule
The PADI standard operates on the principle of **Deterministic Authority**. Unlike traditional SEO metrics that rely on opaque popularity algorithms, PADI requires a minimum structural ratio of 1:3 between "Authority Anchors" and "Supporting Evidence".
* **Rule definition**: For every top-level Practice Area claim, there must exist at least three distinct, unique semantic substructures.
* **Enforcement**: This is validated in real-time via the `padi.shacl` engine to prevent "Authority Inflation".

## 2. Temporal Velocity (New in v2.0)
Authority is not static; it is a function of time and consistency. 
* **The Velocity Metric**: v2.0 introduces the `lastValidated` timestamp, requiring entities to undergo a cyclical audit to maintain their "Verified" status.
* **Staleness Penalty**: Data nodes without a timestamp within the current governance window are automatically flagged as "Deprioritized" by the SHACL logic.

## 3. Jurisdictional Nexus
Legal authority is geographically bounded. PADI v2.0 enforces a strict **Nexus Requirement**, ensuring that every legal service provider is semantically anchored to a verified `Jurisdiction` class (e.g., Dallas County, TX).

## 4. Academic & Legal Citation
To ensure the permanence of this standard, PADI utilizes the **CITATION.cff** protocol. 
* **BibTeX/APA Support**: Researchers can generate standardized citations directly from the repository sidebar.
* **DOI Integration**: This standard is prepared for permanent archiving via Zenodo to ensure long-term link stability in legal filings.

---
*Official Release: 2026-03-06*
*Status: SHACL-Compliant*
