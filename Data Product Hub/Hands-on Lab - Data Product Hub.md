![image](https://github.com/user-attachments/assets/08fb55da-617c-4d25-9be3-9261f6608a8e)# Data Product Hub
IBM Data Product Hub empowers data producers to publish curated data products for easy access by data consumers within their community. This lab introduces the critical features of Data Product Hub, demonstrating its capabilities in data sharing across an organization and automating the delivery of data products for users of all skill levels. Integrating with various source systems, Data Product Hub simplifies the onboarding of data products, regardless of their origin. Data producers can package, operationalize, and share reusable data products such as datasets, AI models, and notebooks. Business users and other data consumers can quickly discover these curated data products and receive them in a format optimized for their needs, reducing friction and improving enterprise data quality, reliability, and discoverability.

# What is a Data Product?
A data product is a composite entity that encapsulates one or more curated data assets designed for reuse and broad distribution. Unlike traditional data assets in governance catalogs, data products are governed through a lifecycle that includes stages such as Draft, Published, and Retired. This lifecycle management ensures that data products are always in a state that maximizes their business value and usability. Data products can include datasets, AI models, notebooks, and more, each thoroughly described with metadata to aid discoverability and usability.

# Key features of Data Product Hub
![image](https://github.com/user-attachments/assets/9bc64ca0-3185-4598-8621-e19cba29e5d2)

# Lab Scenario
Management has observed a decline in order fulfillment rates and increased shipment times, which has resulted in consumer complaints through surveys and customer care channels. To address these concerns, an analytics project has been initiated to conduct a comprehensive investigation to identify the root causes of the significant drop in customer satisfaction over the past year.

To address management's concerns and successfully deliver this project, the following tasks will be performed:
1. Data Product Request
2. Request Acceptance
3. Creation
4. Publish
5. Subscribe and Use

## Personas
### Data Producers
Data Product Hub provides producers with full control over the data product lifecycle. Producers are responsible for creating, publishing, and updating data products to maintain compliance with data quality and security standards. Additionally, producers can enforce governance by defining data-sharing policies and establishing service-level agreements (SLAs) that address access restrictions, delivery mechanisms, and product retirement criteria.

### Data Consumers
Data Product Hub streamlines the process for consumers to find the information necessary to fulfill their business requirements. Consumers can efficiently search through collections of data products and access data from a wide range of sources within a secure environment, thanks to Data Product Hub's integration capabilities with both IBM and third-party tools. The platform also ensures data products are optimized for large-scale sharing across various consumers and consumption endpoints.

**Notes: Username and password will be informed during opening session by mentor**

## Shopping for Data
In this section of the lab, you will assume the role of a Data Consumer. Your task is to find a suitable data product to fulfill a request from management. Specifically, you need to locate a data product that addresses the Employee Effect on Customer Satisfaction use case, which is central to the analytics project. This project aims to identify the root causes of declining customer satisfaction, with a focus on order fulfillment rates and shipment times. To support this investigation, the analytics team requires access to employee and warehouse staff data for decision optimization analysis and enhancements to the executive dashboard.

1. Login as data consumer
   ![image](https://github.com/user-attachments/assets/0454a403-b8d1-4f36-b6fc-880d5dd26b79)

2. Enter Customer as search terms or characters in the search field to discover data products that may uncover insights related to the decline in customer satisfaction.
   Immediately, Customer Demographics and Sales appear, which aligns with the use case. Selects this data product to see if it meets the requirements.
   <img width="1727" alt="image" src="https://github.com/user-attachments/assets/5070198c-348c-46be-9f4e-b81d2c8f994f" />

3. Look through the search results and click on a tile to view the details of a data product.
    A. Verify the business domain & data product contents
   <img width="1728" alt="image" src="https://github.com/user-attachments/assets/d76b2661-2eb4-4280-88d9-f123561dd18c" />

    B. Check the recommended usage
   <img width="851" alt="image" src="https://github.com/user-attachments/assets/0237ed6a-5bbb-42f5-9d7b-5c08d99cc014" />

    C. Assess the data contract to determine its suitability for the analytics project.
   <img width="742" alt="image" src="https://github.com/user-attachments/assets/309fa0e7-269a-4eaf-a3a6-80cdc7d599c9" />

## Requesting a New Data Product
Data Consumers can create a data product request tailored to their specific business needs. In the request, consumers can specify exactly what type of data they need, the format they prefer, and any specific data sources to be used. They can also indicate how they would like the data delivered and how often it should be refreshed. Additionally, they can outline who can access the data and any confidentiality agreements or data retention policies.

Once the request is submitted, producers review the details to make sure they understand the requirements. They might contact the consumers to clarify any points. After confirming the requirements, producers create the data product to meet the specified criteria. When the data product is ready, it is delivered to the consumer in the agreed-upon method, making it available for their business use.

1. Click on the Request a New Data Product button in the top right corner of the screen
   <img width="1728" alt="image" src="https://github.com/user-attachments/assets/433be350-0f72-4c7b-a995-fb3e185f936f" />

2. This will take the requestor to the New data product request form. The requestor must fill out the required fields and click the Submit button to create the request.
   ![image](https://github.com/user-attachments/assets/bf449d08-e3e5-44bd-9e5a-ed4594de6ec1)

3. You also need to fill data contract as it is required for compliance purposes
   <img width="1022" alt="image" src="https://github.com/user-attachments/assets/ccd7d52c-916e-48c4-89d6-9536b0648d5e" />

## Drafting the Data Product
A data product moves through several states that indicate its availability to consumers on the Data Product Hub. The states are: Draft, Published, and Retired.

**Draft**
In the Draft state, the data product is being authored and can be edited as needed. Actions during this phase include adding items, setting the business domain and delivery methods, describing key features and the origin of the data, adding a data contract, and tracking versions by incrementing the version number for each edit. Drafts are listed on the My Work dashboard and can only be edited by the data product owner. A draft data product is not available to the community.

**Published**
Once a data product is published, it becomes accessible to members of the Data Product Hub community. At this stage, the Data Producer can take actions such as restricting access by requiring approval before delivery and adjusting the access level. However, the contents of the data product cannot be modified after publishing. Published data products remain available to the community until they are retired, allowing data consumers to find and subscribe to them.

**Retired**
When a data product is retired, it is no longer available for new subscriptions by consumers and cannot be edited. However, consumers who subscribed before the retirement can continue to work with the data product. Retired data products are not listed on Data Product Hub.

This lifecycle ensures that data products are well-managed and appropriately accessible, maintaining quality and relevance throughout their usage.

1. The Data Producer will need to log into the Data Product Hub.
2. Click the bell icon 🔔 in the top right-hand corner to check for any notifications. Notifications will alert you to new tasks and updates.
   ![image](https://github.com/user-attachments/assets/5a3b1f63-cb8c-454f-8e55-eefad727f4a3)

3. Click the Claim task button to assign the data product request to yourself. This action sends a status update to the consumer, indicating that a producer has viewed and claimed the request.
4. Before approving or rejecting a request, thoroughly read all the requirements and scroll down to the bottom to ensure all details are noticed.
5. Review the request details for each task and choose Approve or Reject. After reviewing the request, the Data Producer decides to approve the task so that they will click the blue accept button in the top right.
   ![image](https://github.com/user-attachments/assets/f5cfcfd2-cdb5-4907-afd6-c07e920e8443)

6. Use the Leave a comment field to message the Data Consumer for further questions or clarifications.
7. Click Submit button
   ![image](https://github.com/user-attachments/assets/2acc7e31-c505-4108-8d0d-f112d297acdf)

8. From the Data Product Hub homepage, select New data product in the upper right-hand corner.
   <img width="1728" alt="image" src="https://github.com/user-attachments/assets/ad82afc6-4ee8-4f8b-b7fb-d3dbaa6eed4d" />

9. Next, the Data Producer will select the source. For this scenario, choose the Add from catalog tile.
    <img width="1244" alt="image" src="https://github.com/user-attachments/assets/b0987c09-4d17-4a44-9f82-be3847744417" />

11. Click on the Select items from the catalog.
    <img width="1232" alt="image" src="https://github.com/user-attachments/assets/548ef372-1a74-4d5f-9259-b2ecf7bad67a" />

12. Here, you can select the items to be added from one or more catalogs. The drop-down menu can be expanded to view more details about each data asset.
   A. EMPLOYEE
   B. EMPLOYEE_RECORDS
   C. CUSTOMER_LOYALTY
![image](https://github.com/user-attachments/assets/89cc89f8-6180-4bfd-936c-17df428cbd73)

13. (If needed) To verify a connection, click the connection status and complete the fields by providing credentials.
    ![image](https://github.com/user-attachments/assets/5434a939-0f84-46e0-8638-f54a1b5dd9bf)

## Completing Data Product
1. Click the Select a business domain button to open the domains list.
   ![image](https://github.com/user-attachments/assets/80595e0a-f0e4-4cb9-bdcf-e46156efe77d)

2. Access levels determine users’ permissions to view, edit, or manage data. Data Producers can choose if data is open to all or requires approval.
   ![image](https://github.com/user-attachments/assets/d3732eed-ed44-4576-8485-cee45531e4a9)

3. Data products are linked to a data contract that sets out the usage terms and conditions. This contract offers assurance to all parties involved when sharing data products across teams.
   ![image](https://github.com/user-attachments/assets/184917ac-d8ca-498b-a374-607c6cd22566)

4. Publish the Data Product
   ![image](https://github.com/user-attachments/assets/af5a1d6a-9920-47d4-879f-008773a344ab)

## Data Product Subscription
In Data Product Hub, consumers can review and subscribe to data products for their business needs. There are two kinds of data products: Unrestricted and Restricted.

**Unrestricted**
Unrestricted data products are Available to all subscribers. When consumers subscribe to a data product, they review the contents, subscribe, and agree to the terms and conditions. After completing the subscription request, they can access the data product by downloading it or opening the URL.

**Restricted**
Some data products are restricted and require approval from an approver designated by the Data Producer. When a data consumer subscribes to a restricted data product, they must provide a business justification and a use case that the approver reviews. If the subscription is approved, the data product is delivered to the consumer through the predetermined delivery method. If the subscription is rejected, the consumer can submit a new subscription with a new business justification.

1. Login as the Data Consumer.
2. The Data Consumer sees a new notification indicating that the Data Producer has completed the data product.
   ![image](https://github.com/user-attachments/assets/b99d2677-d51c-48b7-961f-af98e3c7dcb7)

3. Click on the Employee Effect on Customer Satisfaction card to explore the data product.
   ![image](https://github.com/user-attachments/assets/516fc12a-46ed-43dc-ba98-5918047595a3)

4. Takes a few moments to explore the different parts of the data product to ensure that it meets their requirements from the profile to distribution, as well as exploring the collection of data sets.
   ![image](https://github.com/user-attachments/assets/7d7c44f4-462c-436c-96d2-e8e263fe3d2e)

5. The Data Consumer believes it meets the requirements for the project proposed by management, so they click subscribe.
   ![image](https://github.com/user-attachments/assets/f652d80d-2711-486d-b811-239955fd9e12)

5. Once, the subscription is approved, data consumer will be able to get the data. From the Data Product Hub homepage, select My Subscriptions in the upper right-hand corner.
   ![image](https://github.com/user-attachments/assets/1c9d9692-7f69-4d3f-8784-07a9d5fab998)

6. Once on the Subscriptions dashboard, it can be seen that the Data Producer approved the request and that the data product is delivered. The Data Consumer will now copy the following Flight descriptors in Python and save the code snippets for later use.
   A. CUSTOMER_LOYALTY
   B. EMPLOYEE
   C. EMPLOYEE_RECORDS
   
![image](https://github.com/user-attachments/assets/15b77cb8-cc30-4378-980a-bdf0990440c2)




   
