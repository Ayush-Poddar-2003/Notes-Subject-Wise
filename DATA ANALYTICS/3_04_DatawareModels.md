
#### 1. Enterprise Data Warehouse (EDW)
A comprehensive data repository that integrates data drawn from different areas of an organisation.  
It holds all information for all business units required, 
 giving a consolidated and unified view of the organization.

**Features of Enterprise Data Warehouse (EDW)**
- **Scope and Scale:** The EDWs are deployed for managing data generated from diverse business areas including finance, marketing, selling, and operations.
- **Integration**: It gathers information from transactional databases, ERP systems, CRM systems and other data feeds from outside the business environment.
- **Architecture**: Usually, the structure of an EDW complies with a star/snowflake scheme containing facts (numeric, measurable information) and dimensions (qualitative and contextual data).
- **Usage**: They facilitate complex queries, high-level analysis, and business insight information within the business.
- **Maintenance**: Being central repositories of an organization’s data, EDWs demand investments in infrastructure, upkeep, as well as stewardship for the quality of data kept in them.

----
#### 2. Data Mart
An element of a Data Warehouse system designed  
to hold data from a particular business division, department or user type.  

It is created to serve the specific interests of a specific class of people.

**Features of Data Mart**
- Scope: Data marts are less comprehensive than EDWs and relevant to the organization’s specific departments, such as sales, finance, or marketing.
- Integration: They routinely pull or gather data from the EDW and other operation sources to develop a specific data set.
- Usage: Data marts are used to supply departmental reporting and analysis as the users of this type of data get real-time access to the data that can be useful for their organizational tasks.
- Architecture: Data marts can be deployed based on the star schema or any other simplification of a star-war structure. They can be operations-based or derived (extracted from the operational system directly) or they can be dependent, that is, retrieved from the EDW.
- Flexibility: They also introduce faster implementation and lower cost than building an entire EDW to satisfy all the needs of an organization because they can address departmental requirements instead.

---
#### 3. Virtual Data Warehouse
A Virtual Data Warehouse provides a logical view of data from multiple sources without physically storing the data in a central location.

Features of Virtual Data Warehouses:
- Data Integration: Combines data from various sources without physical movement.
- Real-time Access: Provides up-to-date information directly from source systems.
- Reduced Storage Costs: Minimizes the need for additional storage infrastructure.
- Flexibility: Easily adapts to changes in source systems.