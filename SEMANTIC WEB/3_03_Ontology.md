# Ontology
A formal description of knowledge of a particular domain.  
It includes:
- Concepts (classes)
- Relationships
- Rules
- Constraints
- Axioms (truth statements)
- Reasoning

---
### Why we need Ontology?
To let machines:
- infer (conclude new facts)
- understand relationships
- avoid ambiguity
- share common vocabulary

---
Example Domain: University Ontology

**Classes**:  
Person, Student (subclass of Person), Faculty (subclass of Person), Course

**Properties**:  
teaches, studies, hasID, hasAge

**Rules**:  
A student must study at least one course  
A faculty must teach exactly one course

---
### Benefits of Ontologies  
Machine-understandable meaning  
Data sharing becomes easy  
Avoids inconsistency  
Supports reasoning  
Improves search results  
Good for AI systems  
Reusable knowledge  
Integrates multiple data sources


---

### Challenges of Ontologies

Hard for beginners  
Requires domain expert + technical expert  
Building large ontologies is slow  
Maintaining consistency difficult  
Reasoners become slow on big data  
High learning curve for OWL  
Interoperability issues  

---
### Ontology Design Process 

1. Define the domain
(College, Hospital, Transport)

2. List classes
ex: Person, Student, Course

3. Set up hierarchy
Student → Person
Faculty → Person

4. Define object properties
Student → studies → Course
Faculty → teaches → Course

5. Define data properties
Person → hasAge
Student → hasRollNumber

6. Add restrictions & rules
Student studies at least 1 course
Course must have exactly 1 teacher

7. Add individuals (instances)
Ayush, MCA, BTech

8. Run reasoner
To check logical errors and generate new facts