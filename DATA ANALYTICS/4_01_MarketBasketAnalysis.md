### Market Basket Analysis ?
- Data Mining technique, to identify relationships b/w produts, purchased together in transaction.  
- Based on **Association rule mining**
- To find frequent itemsets & generate association rules.

---
**SUPPORT ?**  
>*Support(X) = (Transactions containing X) / (Total transactions)*  

Higher support → more frequent.

**CONFIDENCE ?**  
>*Confidence(X⇒Y) = Support(X∪Y)/Support(X)* 

How often Y is bought when X is bought.      


**LIFT ?**  
>*Lift = Confidence(X⇒Y)/Support(Y)*   

Measures strength of rule.  
    Lift > 1 = Strong association  
    Lift = 1 = No association  
    Lift < 1 = Negative association

---
### Frequent Itemsets ?
  
>Itemsets with *support ≥ minimum support threshold*

---
### Closed Itemsets

A frequent itemset is closed if **no superset has the same support**.


{milk, bread} appears 10 times  
{milk, bread, butter} also appears 10 times  
So {milk, bread} is NOT closed.

Closed itemsets are useful to reduce number of patterns.

---
### 