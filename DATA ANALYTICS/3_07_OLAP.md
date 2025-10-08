## OLAP ?
- Online Analytical Processing Server
- S/w technology that allows users, to analyze information from multiple database systems at the same time
- Based on multidimensional data model
- OLAP databases are divided into one or more cubes and these cubes are known as Hyper-cubes.


![alt text](image.png)

---
### OLAP OPERATIONS ?

1. **DRILL DOWN** : 
Less detailed into highly detailed data  
It can be done by:
    - Moving down in the concept hierarchy
    - Adding a new dimension
  
    ![alt text](image-1.png)

2. **ROLL UP**
![alt text](image-3.png)

3. **DICE**  
Selecting a sub cube.
![alt text](image-2.png)

4. **SLICE**  
It selects a single dimension, which results in a new sub-cube creation
![alt text](image-4.png) Q1

5. **PIVOT**  
Also known as rotation operation as it rotates the current view to get a new view
![alt text](image-5.png)