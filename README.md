# Basket-Market-Analysis
This project demonstrates how to efficiently collect product data from transactions, apply the **FP-Growth** algorithm for frequent itemset mining using **Apache Spark**, and store the results in a **Neo4j graph database** for easy exploration and analysis.

The data is collected from a **MySQL database**, where each transaction's product details are stored. Spark is then used to scale the **FP-Growth** algorithm to process large datasets efficiently. Finally, the frequent itemsets identified are stored in a **Neo4j graph database** to visualize the relationships between products in the form of a graph.
## Project overflow: 
### 1. Data Collection: 
> Product transaction data is stored in a __MySQL database__. Each row represents a product within a transaction, allowing the dataset to be easily queried and extracted.
### 2. Data Processing :
> - **Apache Spark** is used to process large datasets in parallel and run the FP-Growth algorithm to mine frequent itemsets.
> - **Spark’s MLlib** library is leveraged to apply the FP-Growth algorithm on the transaction data. This ensures the algorithm can scale and handle large amounts of transactional data efficiently.
### 3. Frequent Itemset Mining:
> The **FP-Growth algorithm** identifies frequent product combinations from the transaction data. This step reveals product associations, such as items that are often bought together, which is valuable for marketing strategies and recommendation engines.
### 4. Graph Representation
> The resulting frequent itemsets are stored in a **Neo4j graph database**.
> In Neo4j, products are represented as nodes, and the frequent co-purchases (associations) are represented as edges between these nodes.
> The graph structure allows intuitive exploration and analysis of the product relationships, making it easier to visualize and query for frequent itemsets.
