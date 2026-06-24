# Data Model



The dashboard follows a star-schema-inspired model centered around organizational reporting and GNAF implementation metrics.



#### Dimension Tables

###### 

###### DimOrganization



&#x09;Contains the list of organizations participating in the project.

##### 

##### Fact Tables



###### AllSummary



&#x09;Stores high-level summary metrics for each organization.



###### AllTasks



&#x09;Contains project tasks, progress percentages, and status information.



###### AllServices



&#x09;Contains services/systems and their implementation stages.



###### AllServicesScore



&#x09;Contains GNAF-related scoring metrics, including:



&#x09;    Postal Code Validation



&#x09;    Postal Code Linkage



&#x09;    Inquiry Availability



&#x09;    Security Compliance



###### AllRanking



&#x09;Contains organization ranking metrics.

##### 

##### Relationships



&#x09;DimOrganization is connected to:



&#x20;   		AllSummary



&#x09;        AllTasks



&#x09;	AllServices



&#x09;    	AllServicesScore

&#x09;

&#x20;   		AllRanking



The organization field is used as the primary relationship key across the model.





