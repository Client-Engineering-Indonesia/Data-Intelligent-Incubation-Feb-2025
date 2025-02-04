# Overview Manta Data Lineage
Knowledge Catalog in conjunction with IBM Manta allows data practitioners to augment data assets in a catalog with business metadata, business lineage, and technical data lineage for all stakeholders to understand the provenance of data, how it has changed and moved over time, how it's being used.

<img width="1136" alt="1-overview" src="https://github.com/user-attachments/assets/2adabdbd-d51b-485c-a594-9e5a7484bbf7" />

Business users can view a high-level summary of business lineage and associated metadata: business terms and data quality scores.
Technical users can view advanced data lineage details: technical, indirect, column level, and historical lineage.

<img width="1134" alt="2-overview2" src="https://github.com/user-attachments/assets/1b47e819-da53-4521-b6cc-4b671a785a03" />

# Benefit Manta Data Lineage
Data lineage is an essential component of an effective data management strategy and data governance practice that provides tremendous benefits:

1. Traceability - Where does data originate from, how has it changed over time, how is it being consumed, and by whom
2. Trust in data - Visibility, transparency, and trust into the journey of data to produce accurate and quality analytical and AI outcomes
3. Regulatory compliance - Meet government and industry regulation obligations to truthfully respond to compliance audits and inquires
4. Impact analysis - Assess and understand the downstream impact of planned changes before they negatively impact business processes
5. Root cause analysis - Accelerate data incident identification and remediation by quickly and effectively isolating the cause of the problem
6. Data platform migrations - Sort out the assets that need to be migrated and which ones can be ignored, saving time, money, and resources

# Hands On Lab 
You can try the Manta Data Lineage here https://manta-data-linage-demo.c8f8f055.public.multi-containers.ibm.com
## Get BI Report Lineage

1. Click the New Asset + button. <img width="1136" alt="3-bi_report" src="https://github.com/user-attachments/assets/3f9139e0-ab28-4d5b-8fa9-2bc91b20d161" />

2. Select the Import metadata for data assets task from the Recents section. <img width="1133" alt="4-import_metadataaset" src="https://github.com/user-attachments/assets/c6b0b64c-d455-4e08-8a18-5e3e0209cd75" />

3. Scroll down and select the Get BI report lineage metadata import goal. Click the Next button. <img width="1136" alt="4-import" src="https://github.com/user-attachments/assets/74bab948-d070-4786-a592-141dd5350b37" />

4. Click the Next button. You can skip the description <img width="1137" alt="5-" src="https://github.com/user-attachments/assets/91df496a-0262-4382-ae81-bc3f6848914e" />

5. Select the Executive Dashboard catalog. Click the Next button. <img width="1135" alt="6-" src="https://github.com/user-attachments/assets/fe04b899-3763-40a5-971e-6c8c51b42fb8" />

6. Click the Select scope button. <img width="1134" alt="7-" src="https://github.com/user-attachments/assets/f2b3523e-77d9-4528-ad33-8f30586b6311" />

7. Select the Connection from the Categories list on the left. Select the Team Content folder from the list. Click the Select button. <img width="1137" alt="9-" src="https://github.com/user-attachments/assets/247a6fd3-4433-4e95-bcd6-7dc1de2669d1" />

8. Click the Next button. <img width="1142" alt="10-" src="https://github.com/user-attachments/assets/32a345a4-6a36-4f59-9d26-130f282fe627" />

9. Take the default Job name and leave scheduling turned off. Click the Refresh button on the banner to update the import status. <img width="1136" alt="14-" src="https://github.com/user-attachments/assets/f1732852-2bc5-4754-b457-bfbf4ec328e0" />

10. Click the Next button. <img width="1137" alt="15-" src="https://github.com/user-attachments/assets/ee602e50-c631-4008-9e28-f99e80cd0e47" />

11. Take a minute to review the import. The Scope is importing 1 data asset from the Cognos Analytics connection into the Executive Dashboard catalog as the Target. Click the Create button. <img width="1135" alt="16-" src="https://github.com/user-attachments/assets/5702a417-5097-4002-bb42-8495f9177143" />

12. Click the Refresh button on the banner to update the import status. <img width="1137" alt="17-" src="https://github.com/user-attachments/assets/3fffd545-bd29-40f9-a282-8219230256da" />

13. When the import is complete, a green informational banner will appear with a Metadata import complete message with notification. BI Report lineage imports reports, report queries and a vast amount of report query items (like columns, calculations etc.) depending on how complex the report(s) are that were processed.

    Select the Executive Dashboard project breadcrumb at the top of the page to get back to the project home page. <img width="1136" alt="18-" 
    src="https://github.com/user-attachments/assets/9ae96573-7fb2-4106-9b28-8fa4eb787444" />

## Get ETL Job Lineage
This step creates a Metadata import with a goal of Get ETL job lineage using an IBM Manta scanner to connect to DataStage to collect and document all the technical data lineage for the Executive Dashboard DataStage flow that was created and executed by the data engineer. 

<img width="1135" alt="19-" src="https://github.com/user-attachments/assets/958f48c5-aa5b-42f8-8d5a-e3fa0faf9afc" />

1. Click the New Asset + button. <img width="1137" alt="20-" src="https://github.com/user-attachments/assets/c85acaa3-9578-4a35-879e-7bb78e1d1450" />

2. Select the Import metadata for data assets task from the Recents section. <img width="1137" alt="21-" src="https://github.com/user-attachments/assets/952b35a7-b2ae-4cad-8eaa-8f0ac0a89a58" />
 
3. Scroll down and select the Get ETL job lineage metadata import goal. Click the Next button.<img width="1137" alt="22-" src="https://github.com/user-attachments/assets/6e762327-cce9-46b9-ba59-f0fb13801308" />

4. Click the Next button. You can skip the description <img width="1133" alt="23-" src="https://github.com/user-attachments/assets/2d4033d9-da3c-484c-816b-eee13a181f7f" />

6. Select the Executive Dashboard catalog. Click the Next button. <img width="1138" alt="24-" src="https://github.com/user-attachments/assets/5620a067-7ae8-45fd-84a1-bd90ec480e40" />

7. Click the Select scope button. <img width="1135" alt="25-" src="https://github.com/user-attachments/assets/c3d1a2a3-b505-4fbf-9306-1d67b885c8dc" />

8. Select the DataStage flow category from the Categories list on the left. Select the Executive Dashboard DataStage flow. <img width="1135" alt="26-" src="https://github.com/user-attachments/assets/a9fff8b8-b49c-4b8d-9b14-4b6b4b7c14b6" />

9. Select the Connection category from the Categories list on the left.Select the Arrow on the Db2 connection. Do not select the checkbox. Doing so will select all schemas and tables in the database. <img width="1136" alt="27-" src="https://github.com/user-attachments/assets/e79c1c5d-4213-4dc1-909a-b7239af4787e" />

10. Select the Arrow on the PostgreSQL connection. Do not select the checkbox. Doing so will select all schemas and tables in the database. Select the CUSTOMER schema from the list. <img width="1138" alt="28-" src="https://github.com/user-attachments/assets/d68e5836-b012-420d-8f0c-a89e6a5b7139" />

11. In the schema search area, enter the letters ware to find the WAREHOUSE schema in the list. Select the WAREHOUSE schema from the list. <img width="1138" alt="29-" src="https://github.com/user-attachments/assets/4e206e4d-94cf-45cd-9bd6-5bb6dc01fde6" />

12. Before continuing, review the scope selections and make sure the DataStage flow, Db2 CUSTOMER and OUTCOMES schemas and the PostgreSQL CUSTOMER and WAREHOUSE schemaS are included in the scope. Click the Next button. <img width="1136" alt="41-" src="https://github.com/user-attachments/assets/89595eb6-1be3-4b57-a5db-61a76ce84080" />

13. Take the default Job name and leave scheduling turned off. Click the Next button. <img width="1136" alt="42-" src="https://github.com/user-attachments/assets/9d11a86a-fe58-412a-85b7-5318e4a58df9" />

14. Take the default Advanced options that are selected for the Update on reimport options. Click the Next button <img width="1137" alt="43-" src="https://github.com/user-attachments/assets/0f30f50e-4770-4028-bff8-6680cf7f3548" />

15. Click the Create button. <img width="1135" alt="44-" src="https://github.com/user-attachments/assets/2046641d-40c2-41f7-a846-988097b24222" />

    An error message box might appear in the top right corner that looks like the screen shot below saying the Metadata Import asset with this name already exists. This is a known defect that has been reported to development <img width="1135" alt="45-" src="https://github.com/user-attachments/assets/e066505e-81d8-4ccb-a473-4a54e7c56783" />

    Add a suffix like v2 to the end of the name. Click the Next button 4 times to the last page of import wizard that has the Create button <img width="1135" alt="46-" src="https://github.com/user-attachments/assets/488adc9a-518b-4693-a55a-b45148674cfb" />

16. Click the Refresh button on the banner to update the import status. <img width="1136" alt="47-" src="https://github.com/user-attachments/assets/6e91066b-d77c-4b80-80f3-968e3d53f3f3" />

30. When the import is complete, a green informational banner will appear with a Metadata import complete message with notification. 
    ETL Job lineage imports data integration jobs, stages, tables and files that are source and target dependencies, and a vast amount of data     
    integration columns depending on how complex the data integration job is and how many dependencies there are that were processed. <img width="1138" alt="48-" src="https://github.com/user-attachments/assets/ff12d443-47dd-4192-9242-08baf7b38fda" />


## Review Lineage Results
1. 
<img width="1136" alt="49-" src="https://github.com/user-attachments/assets/2895b93c-ecc8-4cca-a4e7-8d5e62c8fa41" />

2. 
<img width="1136" alt="50-" src="https://github.com/user-attachments/assets/ae2d3e04-2409-4578-b791-eb234c7aa43e" />

3. 
<img width="1134" alt="51-" src="https://github.com/user-attachments/assets/5c4e1648-e500-484e-ae6c-c6721e438b66" />

4. 
<img width="1134" alt="52-" src="https://github.com/user-attachments/assets/d4bdc6d5-bea4-4a5e-921f-63903f3d200b" />

5. 
<img width="1135" alt="53-" src="https://github.com/user-attachments/assets/b19e63b0-90e9-4440-ab7a-d655fbff901f" />

6.
<img width="1136" alt="54-" src="https://github.com/user-attachments/assets/a38aa2d8-9f0e-4b45-8770-f511c0481362" />

## Review ETL Job Lineage

1. 
<img width="1138" alt="55-" src="https://github.com/user-attachments/assets/e3443e57-a330-4061-b19d-7609533353ec" />

2. 
<img width="1136" alt="56-" src="https://github.com/user-attachments/assets/3b9d235b-d208-4338-9383-5eb6563097ef" />

3. 
<img width="1134" alt="57-" src="https://github.com/user-attachments/assets/fe161630-97bc-4736-94ed-ed57e98f851d" />

4.
<img width="1137" alt="58-" src="https://github.com/user-attachments/assets/45b8212c-b12a-42d5-b0a7-4c6ac90a1973" />

5.
<img width="1137" alt="59-" src="https://github.com/user-attachments/assets/3c9c04aa-402b-4197-ae52-132eefbc7dca" />

6.
<img width="1137" alt="60-" src="https://github.com/user-attachments/assets/14c37b60-be9d-4b43-a2e8-c2d17e0f7ccf" />

7.
<img width="1138" alt="61-" src="https://github.com/user-attachments/assets/5efaf428-0b1a-48d8-afd8-7ce9e9a904bd" />

8.
<img width="1136" alt="62-" src="https://github.com/user-attachments/assets/f7e275cf-b4e9-4030-88cc-3fe239227f9c" />

9.
<img width="1134" alt="63-" src="https://github.com/user-attachments/assets/41442c19-6fba-497d-ba5a-b840424b00de" />

10.
<img width="1136" alt="64-" src="https://github.com/user-attachments/assets/877799ef-048c-4a70-b28c-43a85c0d6cb2" />

11.
<img width="1136" alt="65-" src="https://github.com/user-attachments/assets/4cb0e01a-2603-4097-a770-31c931ef0dcf" />

12.
<img width="1136" alt="66-" src="https://github.com/user-attachments/assets/19952800-7599-4fa8-aa4f-8cf0287eb600" />

13.
<img width="1137" alt="67-" src="https://github.com/user-attachments/assets/6eac6e83-d705-4d8a-bb72-34f8b80df8bc" />

14.
<img width="1136" alt="68-" src="https://github.com/user-attachments/assets/b278b3d7-a9fb-4b92-a5a2-c3707f80b5f7" />

15.
<img width="1137" alt="69-" src="https://github.com/user-attachments/assets/bc979ed4-c502-4dca-b34e-049c92cc1c96" />

16.
<img width="1137" alt="70-" src="https://github.com/user-attachments/assets/eceb5196-469c-4616-9d1f-48f6af802415" />

17.
<img width="1136" alt="71-" src="https://github.com/user-attachments/assets/4a03e7b1-440c-4ad9-a5f3-be76733b14e9" />

18.
<img width="1134" alt="72-" src="https://github.com/user-attachments/assets/405f0f1e-60da-4e55-9bb1-b70d6842065a" />

19.
<img width="1136" alt="73-" src="https://github.com/user-attachments/assets/0162c749-21d9-42d0-b218-75e66776dc63" />

20.
<img width="1137" alt="74-" src="https://github.com/user-attachments/assets/59e817f4-0dc5-478f-8706-09780a385de8" />

21.
<img width="1137" alt="75-" src="https://github.com/user-attachments/assets/cbb20745-c579-4dbd-ad56-abe9ed0f4d0c" />

22.
<img width="1136" alt="76-" src="https://github.com/user-attachments/assets/a28b52f7-e762-4f47-b749-a115977a114a" />

23.
<img width="1134" alt="77-" src="https://github.com/user-attachments/assets/df50d0dd-bc67-475a-8f3d-b27c03cc8b6e" />

24.
<img width="1136" alt="78-" src="https://github.com/user-attachments/assets/303b445d-54ac-47b0-995b-f1c5c609919e" />

25.
<img width="1136" alt="79-" src="https://github.com/user-attachments/assets/48c9277f-b5b7-4713-84ae-b7452d06442d" />

26.
<img width="1135" alt="80-" src="https://github.com/user-attachments/assets/c056190b-0a03-4899-83b3-29f6a181b431" />

27.
<img width="1135" alt="81-" src="https://github.com/user-attachments/assets/750ac20d-a8a6-481f-815d-03834b4f0bcc" />


## Review BI Report Lineage
1. 
<img width="1135" alt="82-" src="https://github.com/user-attachments/assets/c98c57f6-ded7-4286-9f86-7dafa6ab3505" />

2. 
<img width="1136" alt="83-" src="https://github.com/user-attachments/assets/bed4e282-93ca-41ec-a55d-0b6e07da36c2" />

3.
<img width="1137" alt="84-" src="https://github.com/user-attachments/assets/9d86b4aa-47a4-4a4e-869e-39668faa0c16" />

4.
<img width="1136" alt="85-" src="https://github.com/user-attachments/assets/009bf7e7-eeea-49d3-be06-55368572cf0a" />

5.
<img width="1136" alt="86-" src="https://github.com/user-attachments/assets/29a83fd8-2dd3-4d43-a0cc-5e2cbad9227e" />

6.
<img width="1135" alt="87-" src="https://github.com/user-attachments/assets/19e2987a-6331-4ae7-ba85-747637f7e8c8" />

7.
<img width="1136" alt="88-" src="https://github.com/user-attachments/assets/506a136e-3a59-4779-9ea9-e8270fb35ccc" />

8.
<img width="1138" alt="89-" src="https://github.com/user-attachments/assets/09b83d81-bca2-4860-b68d-27a91029a31c" />

9.
<img width="1136" alt="90-" src="https://github.com/user-attachments/assets/77de7e19-9c99-46c9-9692-81d4f11589b1" />

10.
<img width="1135" alt="91-" src="https://github.com/user-attachments/assets/f3f509db-64c3-48ca-a8c5-cb2ef18b52c0" />

11.
<img width="1135" alt="92-" src="https://github.com/user-attachments/assets/e7333502-8bfb-4cb1-bb52-9505df848a39" />

12.
<img width="1136" alt="94-" src="https://github.com/user-attachments/assets/312313d7-eb44-4309-a8fe-983e9a2a13ee" />



