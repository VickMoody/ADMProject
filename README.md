# ADMProject
Advanced Data Management Project with Neo4j

To execute the codes you need Neo4j.
1.create a new project in Neo4j
2.create a new database inside that project (do not run)

(choose only 1 option in step 3 --- automatic import or --- manual ctrl-c + ctrl+v)

3. ----- MANUAL COPY PASTE (Faster) --------------------------------------------------------
4. run the database and open a Neo4j browser
5. open the crimegraph.cypher from codes directory and copy load and other queries one by one into command line inside browser(In the same order)
(or import directly into cypher)

--------------------------------------------------------------------------------------------

OR

3. ----- AUTOMATIC IMPORT OF CYPHER ---- TAKES SOME TIME (~30min - be patient) -------------------
4. install APOC plugin (you can find it in plugins window of the database)
5. Inside settings window add (conf file of your database neo4j.conf):
apoc.export.file.enabled = true
apoc.import.file.enabled = true
6. copy dbexport.cypher into your Neo4j directory of the created database
(in our case it is C:\Users\Victoria\AppData\Roaming\Neo4j Desktop\Application\neo4jDatabases\database-239b317d-5c98-4550-989f-b4e86be5c9f1\installation-3.3.3\)
7. run the database and open a Neo4j browser
8. execute inside command line:
call apoc.cypher.runFile('dbexport.cypher');
--------------------------------------------------------------------------------------------


Your graph is ready to use!

To execute queries on the created database:
open file queries.cypher from codes directory
and copy a query into command line one by one to see the results.
