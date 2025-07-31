# RequirementsOntology
Software system designers are always faced with the problem of extracting requirements, both functional and non-functional. 
To solve this problem, the use of ontology has been proposed. The present ontology is designed to extract software requirements, both functional and non-functional, of an online sales system.
This ontology is designed using Protege software version 5.5.0 beta. To use it, you need to open this ontology with this software. 
To view the classes, use the classes tab. Requirements are mapped as properties between classes and you can add new requirements and use them in the future.
A domain and a range are introduced for each relationship. Then an instance is created for each class and the relationships are repeated for these instances.
To view the specified requirements for a class, use the DL Query tab. 
In the opened page, you can use the name of your instance or class, after activating Reasoner from Reasoner tab, and selecting Pallet as the analyzer, check the boxes you need from the right side of the system. Then click the execute button to complete the analysis and display.
To view all items using SPARQL, you can use the following code snippet. Type this code snippet in the SPARQL Query tab and click the execute button at the bottom of the page.
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
SELECT ?individual ?type
WHERE {
?individual a ?type .
}
To view the number of extracted requirements, use the following SPARQL code as before.
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
SELECT (COUNT (DISTINCT ?p) AS ?totalProperties)
WHERE {
?pa owl:ObjectProperty
}
For any other questions, you can contact us via the email below and receive your answer.
Houbakht.Attaran@iau.ir

