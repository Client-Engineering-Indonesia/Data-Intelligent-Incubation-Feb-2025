# Follow the steps described below

Table of contents:
1. [Personas and their roles](https://github.com/Client-Engineering-Indonesia/Data-Intelligent-Incubation-Feb-2025/blob/main/IBM%20Knowledge%20Catalog/Hands-on%20Lab%20-%20IBM%20Knowledge%20Catalog.md#section1)
2. [Connect your data sources](https://github.com/Client-Engineering-Indonesia/Data-Intelligent-Incubation-Feb-2025/blob/main/IBM%20Knowledge%20Catalog/Hands-on%20Lab%20-%20IBM%20Knowledge%20Catalog.md#section2)
3. [Define Business Vocabulary](https://github.com/Client-Engineering-Indonesia/Data-Intelligent-Incubation-Feb-2025/blob/main/IBM%20Knowledge%20Catalog/Hands-on%20Lab%20-%20IBM%20Knowledge%20Catalog.md#section3)
4. [Curate and enrich data assets](https://github.com/Client-Engineering-Indonesia/Data-Intelligent-Incubation-Feb-2025/blob/main/IBM%20Knowledge%20Catalog/Hands-on%20Lab%20-%20IBM%20Knowledge%20Catalog.md#section4)
5. [Catalog Governed Data](https://github.com/Client-Engineering-Indonesia/Data-Intelligent-Incubation-Feb-2025/blob/main/IBM%20Knowledge%20Catalog/Hands-on%20Lab%20-%20IBM%20Knowledge%20Catalog.md#section5)

<h1 id="section1">1. Personas and their roles</h1>

| Role | Responsibilities |
| --   |       ---        |
| Data Steward  | 1. Define and publish a complete and meaningful set of business vocabulary **governance artifacts**. <br> 2. Create the **governance rules** that were required by the governance policy that protects sensitive information.<br> 3. Create the **data protection rules** to protect personal and sensitive information based on the approved governance policies and rules.<br> 4. Discover and **import the data assets** that were needed using the Metadata Import tool. <br> 5. Curate the data assets using the **Metadata enrichment** tool to profile, access data quality, and assign business terms and data classes.<br> 6. **Publish the connections and data assets** to a governed catalog.<br> 7. **Augment the cataloged assets** with additional metadata: Tags, Classifications, Related Assets, and Reviews.  |
| Privacy Steward | **Review and approve** the governance policies and rules.|
| Quality Analyst | 1. **Assess** data quality issues and **create a data quality definition** and data quality rules.<br> 2. **Create a Data Quality SLA remediation rule** to monitor data quality issues that invokes the data quality SLA remediation workflow.|
| Business User (Data Scientist) | **Find the data they need** and review the catalog assets and metadata. |

Other than the roles mentioned above, there is another role responsible for managing system configuration, which is the Administrator. In this use case, this role is responsible for:
1. Defining the roles --such as Data Steward, Privacy Steward, Quality Analyst, and Business User--, setting permissions for each role, and assigning roles to users;
2. Defining the data sources that contain the relevant data needed by the project team.

<h1 id="section2">2. Connect to data sources</h1>
The very first step in your journey to establishing Data Intelligence in your organization is to identify all data sources within your company and establish connections to those systems. This step is ideally performed by the Administrator or Senior Data Stewards. Some large organizations grant each data owner (producer) access to their Knowledge Catalog, allowing them to connect their data sources independently.

Before the data governance lifecycle processes can begin, data stewards and data consumers need access to data. As a best practice, identifying and providing access to data sources needs to happen before data stewardship can begin so that the data is accessible to the data steward to begin discovering relevant data, analyzing data content and quality, and enforcing data privacy policies in order to provide timely access to high quality, governed data to the data consumers who will use it for analytics and AI.

Goals:
- [ ] Check platform connections provided by Administrator

Steps
1. Login as Data Steward using the assigned username and password. 
2. Select Data > Connectivity from the menu
![image](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image4.png)
3. You will see 3 available connections on platform level that have been created by the Administator.
![List of platforms connections](images/platform_connections.png)

<h1 id="section3">3. Define Business Vocabulary</h1>

This section creates all the governance artifacts needed to establish a trusted, business ready, governance foundation. It uses a set of CSV files to import and create the artifacts in the upcoming steps so make sure the governance artifacts zip file has been downloaded and unzipped. Download here: [Data Cataloging and Governance](https://github.com/CloudPak-Outcomes/Outcomes-Projects/blob/main/Knowledge-Catalog-L4-PoX-Lab/Knowledge-Catalog-L4-PoX-Lab.zip)

It is essential to establish the business vocabulary first before any data curation, enrichment and cataloging of data assets takes place. This is because governance artifacts, like data classes and business terms, can be automatically assigned to data assets during metadata enrichment and cataloging. If not, all of those tasks would have to be done manually, which defeats taking advantage of the automated and built-in data governance capabilities of Knowledge Catalog.

#### 1. Create custom properties
Custom properties and relationships need to be defined before any data governance artifacts are defined because they will be attributes of those governance artifacts and need to be established before the artifacts are imported and created. 

Goal: 
- [ ] Create a custom property, called Department, that will be added to all business terms. 

Steps
1. Select the Navigation menu (the 4 stacked horizontal lines in the upper left corner).
2. Select Administration > Governance and catalogs from the menu.
![section3_1](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image20-35.png)
3. Select the `Asset and artifact definitions` tile.
4. Select the `Custom properties` definition from the left side menu.
5. Click the `Import from file` button.
![section3_2](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image20-37.png)
6. Click the `Drag and drop file here or upload` link.
7. Select the `governance-custom-attributes.json` file from your download location.
8. Click the `Open` button.
![section3_3](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image20-39.png)
9. Click the `Import` button.
10. A message box will appear with a notification that 1/1 custom attributed was imported successfully.
![section3_4](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image20-41.png)


#### 2. Create categories
Categories act as folders or directories to organize governance artifacts and provide access controls to authorize who can author and manage those artifacts. Categories provide the logical structure for all governance artifacts, except data protection rules. You group governance artifacts in categories to make them easy to find and manage, and to control their visibility. Categories can be organized in a hierarchy based on their meaning and relationships to one another. A category can have subcategories, but a subcategory can have only one direct parent category.

In this section, 3 categories will be imported and created (one parent category and two sub-categories) that will provide the logical structure for the governance artifacts that are defined in this lab.

Goals:
- [ ] sa

Steps
1. Select the Navigation menu (the 4 stacked horizontal lines in the upper left corner).
2. Select `Governance` > `Categories` from the menu.
![section3_5](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image21.png)
3. Using the `Add category` dropdown, select `Import from file`.
![section3_6](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image22.png)
4. Click the `Drag and drop file here or upload` link.
5. Select the governance-categories.csv file from your download location.
6. Click the `Open` button.
![section3_7](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image24.png)
7. Click the `Next` button.
8. Select the `Replace all values merge` option. NB: If you 
9. Click the `Next` button.
![section3_8](https://cp4d-outcomes.techzone.ibm.com/img/l4-pox/knowledge-catalog/image26.png)
10. Select the `Close` button.


#### 3. Create classifications 

#### 4. Create reference data

#### 5. Create data classes

#### 6. Create business terms

<h1 id="section4">4. Curate and enrich data assets</h1>

- create project 
- review available connections
<img width="1244" alt="image" src="images/section4_1.png" />

- import data assets
- enrich data assets
- review asset enrichment
- review column enrichment
- rectify 

<h1 id="section5">5. Catalog Governed Data</h1>

- create catalog
- publish connection
- publish data assets
- augment postgreSQL
- augment Employee Metadata


6. Define Policies and Rules
- Define workflow for data privacy
- create governance policy
- create governance rules 
- approve as privacy steward
- create date of birth rule
- create email address rule
- Approve as Privacy Steward

---
7. Manage Data Quality 
- data quality remidiation workflow
- review quality result
- add db2 connection 
- create data quality definition
- create data quality Rule
- create data quality SLA rule
- activate SLA rule monitoring

---
8. Discover Data
- Find the right data
- review featured assets
- review employee data

---
9. About IBM Knowledge Accelerator


