# Autolabeling-Opexwise
Created multiple labels automatically for documents containing at least 50,000 rows each. Grouped them into top 50 labels identified through NLP processes and Topic Modeling.


## Steps to build the KNOWLEDGE GRAPH:

1. Preprocess the unstructured text. Follow the steps in the kg_pipeline.ipynb. Please run pip install -r requirements.txt to install all the dependencies.

2. Create Semantic Triples (Subject, Verb, Object) for each row of the data.

3. Create a TypeDB database once you've installed TypeDB on your system and started the server.

4. Create a SCHEMA for the database. Look at kgSchema.tql for example.

5. Use Python/Java/NodeJS as a client to access TypeDB API. In this case Python has been used.
 
6. Connect to the typedb server and transfer the data from python to typedb.

7. Install TypeDB Studio and connect to the server and database.

8. Use match $x isa thing; to see the snapshot of the entire knowledge graph. Or, open Visualize_KG.tql using TypeDB Studio.

