# PADI Technical Standard v2.0
**The Practice-Area Depth Index for Legal Authority Architecture**

Welcome to the official technical documentation for PADI. This standard provides a deterministic framework for measuring legal authority using OWL 2 Ontologies and SHACL validation logic.

## 🏛️ Core Components
* **[Master Taxonomy](./padi.ttl)**: The formal RDF/OWL definitions of legal practice areas.
* **[Validation Logic](./padi.shacl)**: The SHACL shapes enforcing the "1003 Cardinality Rule."
* **[Citation Specification](./CITATION.cff)**: Standards for academic and legal referencing.

## 🚀 Quick Start for Engineers
To validate a law firm dataset against the PADI v2.0 standard:
```bash
pyshacl -s padi.shacl -m human -f table padi.ttl
