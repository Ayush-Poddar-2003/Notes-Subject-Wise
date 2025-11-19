# SPARQL

SQL is for relational DB.  
SPARQL is for RDF data graph

---
### SPARQL Concerns / Limitations
- Slow on huge graphs
- Needs indexing for good performance
- Complex syntax for non-tech users
- Hard debugging for large queries
- Requires standard URIs and consistent ontology
- Query results depend on correct ontology design

---
### Tools for SPARQL
1. **Protégé (with SPARQL plugin)**  
Can run SPARQL inside ontology  
Export data  
Test ontology results

2. **Twinkle**  
A simple SPARQL query tool  
Connect to RDF files or endpoints  
Good for debugging SPARQL

3. **Apache Jena + Fuseki**  
Enterprise level  
Used for SPARQL endpoints  
Used in production Semantic Web projects