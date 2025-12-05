Similarity  
Numerical measure of how alike two data objects are  
Value is higher when objects are more alike  
Often falls in the range [0,1]


Dissimilarity (e.g., distance)  
Numerical measure of how different two data objects are  
Lower when objects are more alike  
Minimum dissimilarity is often 0  
Upper limit varies

Proximity refers to a similarity or dissimilarity

---

### DATA MATRIX
Normal matrix  
Rows = objects, Columns = attributes

### DISSIMILARITY MATRIX
Square matrix  
Entry (i, j) = distance/similarity between objects i & j  
hence diagonal remains 0  

> **Similarity( i, j ) = 1 - dist( i, j )**

---

## <center> PROXIMITY ATTRIBUTES

#### 1. NOMINAL 
If disimilarity = 1 => Completely different  
and if 0 => completely same  
![alt text](image-36.png)
![alt text](image-38.png)
![alt text](image-37.png)

---

#### 2. BINARY ATTRIBUTES
![alt text](image-39.png)

iF ![alt text](image-40.png)  
![alt text](image-41.png)
![alt text](image-42.png)

---
Asymmetric : ![alt text](image-43.png)

Symmetrix : ![alt text](image-44.png)

---

#### 3. NUMRICAL ATTRIBUTES

![alt text](image-45.png)  
![alt text](image-46.png)

---
#### 4. ORDINAL ATTRIBUTE

Convert ranks to [0, 1] scale.

![alt text](image-47.png)  
![alt text](image-48.png)

Total states : ![alt text](image-50.png)

![alt text](image-49.png)

Similarly every ![alt text](image-51.png)