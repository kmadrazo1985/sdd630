<br><br>
<h2 align="center">Activity 6</h2>
<br><br>

<h4 align="center">Kenia Madrazo</h4>
<h4 align="center">Grand Canyon University</h4>
<h4 align="center">CET</h4>
<h4 align="center">SDD-630</h4>                     
<h4 align="center">Professor Bobby Estey</h4>
<br><br>                  
<br><br>

<h3><p style="text-align: justify; margin-left: 3.5em; margin-right: 3.5em;">Evaluating Data Storage Options: Strengths, Weaknesses, and Application Recommendations</h3>

<h3><p style="text-align: justify; margin-left: 3.5em; margin-right: 3.5em;">Introduction</h3>
<p style="text-align: justify; text-indent: 4.5em; margin-left: 3.5em; margin-right: 3.5em;">
&emsp;&emsp;The landscape of data storage has expanded rapidly in recent years due to the explosion of mobile, web, and distributed applications. Modern systems deal with various data types, including structured records, unstructured content, logs, and relationships among entities. As a result, developers and architects must choose storage technologies suited to their specific needs rather than relying solely on traditional relational databases. This paper examines four major categories of databases relational, document, graph, and search engine highlighting their respective strengths, weaknesses, and ideal use cases. The conclusion includes a recommendation tailored to a mobile application project, such as KenHealthPost, focused on mental wellness and user interaction
</p>


<h3><p style="text-align: justify; margin-left: 3.5em; margin-right: 3.5em;">1. Relational Databases (RDBMS)</h3>
<p style="text-align: justify; text-indent: 4.5em; margin-left: 3.5em; margin-right: 3.5em;">
&emsp;&emsp;Relational databases like MySQL, PostgreSQL, and Microsoft SQL Server store data in tabular form using a predefined schema. Data access relies on Structured Query Language (SQL), and relationships between tables are enforced using primary and foreign keys (Coronel & Morris, 2015).

**Strengths:**

&emsp;&emsp;✔️Data Integrity: Strong adherence to ACID (Atomicity, Consistency, Isolation, Durability) principles ensures high data reliability.

&emsp;&emsp;✔️Structured Querying: SQL enables precise and powerful data retrieval operations.

&emsp;&emsp;✔️Mature Ecosystem: Decades of development have led to stable, well-supported systems with strong community and vendor support.

&emsp;&emsp;✔️Normalization & Joins: Excellent for complex queries involving normalized data and relationships between multiple entities.

**Weaknesses:**

&emsp;&emsp;🔻Rigid Schema: Any changes to the schema require migrations, which can be complex in dynamic or evolving applications.

&emsp;&emsp;🔻Horizontal Scaling: Scaling relational databases across multiple servers is difficult and often requires sharding or expensive clustering solutions.

&emsp;&emsp;🔻Join Performance: Queries involving multiple joins can be slow on large datasets unless heavily optimized.

**Use Cases and Example:**
Relational Database Management Systems (RDBMSs) are ideal for applications that require structured, consistent, and real-time access to data, especially in environments where multiple users need to read and write critical information simultaneously. In a networking platform like KenHealthPost, where mental health specialists must frequently access, update, add, delete and securely share patient records, relational databases provide the transactional integrity, concurrency control, and strong data relationships necessary to ensure accuracy and compliance.

Features such as messaging between users, appointment tracking, role-based access, and patient history management rely heavily on the reliability and consistency of relational data models. Relational databases ensure that all users, patients, specialists, and administrators interact with up-to-date information without conflicts or data loss, even when multiple updates occur simultaneously.

<h3><p style="text-align: justify; margin-left: 3.5em; margin-right: 3.5em;">2. Document Databases (NoSQL)</h3>
<p style="text-align: justify; text-indent: 4.5em; margin-left: 3.5em; margin-right: 3.5em;">
&emsp;&emsp;Document databases such as MongoDB and Couchbase store data as JSON, BSON, or XML documents. These are semi-structured and self-contained, allowing each document to differ in structure (MongoDB, n.d.).

**Strengths:**

&emsp;&emsp;✔️Schema Flexibility: Allows each document to have its own unique fields, making it suitable for evolving applications.

&emsp;&emsp;✔️Horizontal Scalability: Designed to scale out easily using distributed nodes.

&emsp;&emsp;✔️Embedded Data Model: Related information can be stored together in one document, improving performance by avoiding joins.

&emsp;&emsp;✔️Agile Development: Developers can iterate faster without needing to update schemas with every change.

**Weaknesses:**

&emsp;&emsp;🔻Data Duplication: Denormalized data can lead to inconsistencies if updates are not managed properly.

&emsp;&emsp;🔻Weaker Transactional Support: Although recent versions support multi-document ACID transactions, it's not as mature as in RDBMS.

&emsp;&emsp;🔻Poor for Complex Relationships: Many-to-many relationships are not efficiently handled due to the lack of joins.

**Use Cases and Example:**
Popular among startups and mobile app developers, document databases work well in content management systems, messaging apps, and real-time analytics. Spotify uses MongoDB to store dynamic user data such as playlists, preferences, and listening history (Pearson, 2013).

<h3><p style="text-align: justify; margin-left: 3.5em; margin-right: 3.5em;">3. Graph Databases</h3>
<p style="text-align: justify; text-indent: 4.5em; margin-left: 3.5em; margin-right: 3.5em;">
&emsp;&emsp;Graph databases such as Neo4j and Amazon Neptune model data as nodes and edges, which represent entities and their relationships. They are optimized for querying interconnected data (Robinson, Webber, & Eifrem, 2015).

**Strengths:**

&emsp;&emsp;✔️Optimized for Relationships: Perfect for traversing multiple levels of connections quickly.

&emsp;&emsp;✔️Flexible Schema: Nodes and relationships can easily be modified or extended.

&emsp;&emsp;✔️Query Language: Languages like Cypher provide expressive power for relationship-heavy queries.

**Weaknesses:**

&emsp;&emsp;🔻Limited General Use: Not ideal for flat, tabular data or bulk processing.

&emsp;&emsp;🔻Scaling Complexities: Large-scale graph traversals may require careful partitioning and are harder to scale horizontally.

&emsp;&emsp;🔻Less Adoption: Fewer developers are familiar with graph databases, and tooling is still growing.

**Use Cases and Example:**
Commonly used in social networking, fraud detection, and recommendation engines. LinkedIn and Facebook use graph databases to analyze and model user connections for friend suggestions and content personalization (Neo4j, n.d.).

<h3><p style="text-align: justify; margin-left: 3.5em; margin-right: 3.5em;">4. Search Engine Databases</h3>
<p style="text-align: justify; text-indent: 4.5em; margin-left: 3.5em; margin-right: 3.5em;">
&emsp;&emsp;Search engine databases like Elasticsearch and Apache Solr index data for fast retrieval and powerful full-text search. They are designed for querying large amounts of textual and semi-structured data (Elastic, n.d.).

**Strengths:**

&emsp;&emsp;✔️Full-Text Search: Offers powerful text processing features such as stemming, fuzzy matching, and relevance scoring.

&emsp;&emsp;✔️Real-Time Analytics: Enables faceted navigation and statistical aggregation of data.

&emsp;&emsp;✔️Horizontal Scaling: Built for distributed, fault-tolerant environments.

&emsp;&emsp;✔️Integration-Friendly: Often used alongside relational or NoSQL databases for search-specific tasks.

**Weaknesses:**

&emsp;&emsp;🔻Not Transactional: Lacks native support for multi-step transactions.

&emsp;&emsp;🔻Data Duplication: Requires synchronization with other systems.

&emsp;&emsp;🔻Operational Complexity: Index tuning and configuration can be technically demanding.

**Use Cases and Example:**
Used in e-commerce search, log aggregation, and document retrieval. For example, eBay uses Elasticsearch for its fast, user-friendly product search and filtering capabilities (Pearson, 2013).

<h3><p style="text-align: justify; margin-left: 3.5em; margin-right: 3.5em;">5. Recommendation for Mobile Application</h3>
<p style="text-align: justify; text-indent: 4.5em; margin-left: 3.5em; margin-right: 3.5em;">
&emsp;&emsp;For a mobile app like KenHealthPost, which serves mental health professionals and patients with features such as user profiles, posts, appointments, and messaging, a relational database is the most suitable primary data storage solution.

✔️ Primary Database: Microsoft SQL Server
SQL Server is a powerful enterprise-grade relational database that provides a structured and highly secure environment, which is essential for handling sensitive healthcare data. Its support for ACID transactions, foreign key constraints, and indexed views ensures high data integrity, consistency, and performance crucial for features such as appointment scheduling, role-based access control, and medical history tracking. Additionally, SQL Server's built-in security features like row-level security, dynamic data masking, transparent data encryption (TDE), and auditing tools help meet stringent data privacy and compliance standards such as HIPAA and GDPR.
Tight integration with .NET Core and Entity Framework makes SQL Server an ideal match for the KenHealthPost platform, streamlining development and improving maintainability.

✔️ Search Layer: Elasticsearch (Optional)
For advanced search features such as full-text search, autocomplete, and relevance-based filtering across posts, messages, or community resources, Elasticsearch can be integrated as a dedicated search engine. While SQL Server does offer full-text indexing, Elasticsearch is optimized for complex search use cases and large-scale content retrieval.

✔️ Graph Layer: Neo4j(Optional)
If future versions of KenHealthPost introduce social or professional networking features such as patient-provider matching, connection graphs, or personalized recommendations, Neo4j can be used in conjunction to efficiently model and query relationship-driven data.

## Conclusion
&emsp;&emsp;Each database technology offers strengths tailored to specific storage and access patterns. While document databases excel in handling flexible, semi-structured data, and graph databases are well-suited for managing complex relationships, relational databases remain the gold standard for applications that require structured data, transactional integrity, and real-time multi-user access.

&emsp;&emsp;For a modern mobile application like KenHealthPost, where mental health professionals must continuously access and update sensitive patient records, and where features like messaging, appointments, and role-based permissions demand consistency and reliability, a relational database such as SQL Server provides the ideal foundation. Its support for ACID transactions, strong security mechanisms, and seamless integration with the .NET ecosystem ensures data accuracy, privacy, and compliance.

&emsp;&emsp;To enhance specific features such as intelligent search or future social networking capabilities, technologies like Elasticsearch and Neo4j can be integrated as complementary layers. However, the core architecture should rely on the proven strength and structure of a relational database, ensuring scalability, maintainability, and trust in handling mission-critical data.

## References

Coronel, C., & Morris, S. (2015). Database Systems: Design, Implementation, & Management (11th ed.). Cengage Learning.
Elastic. (n.d.). What is Elasticsearch? Retrieved from https://www.elastic.co/elasticsearch
MongoDB. (n.d.). What is MongoDB? Retrieved from https://www.mongodb.com/what-is-mongodb
Neo4j. (n.d.). Neo4j Use Cases. Retrieved from https://neo4j.com/use-cases/
Pearson, T. (2013). Database Design and Implementation. Pearson Education.
Robinson, I., Webber, J., & Eifrem, E. (2015). Graph Databases: New Opportunities for Connected Data (2nd ed.). O’Reilly Media.