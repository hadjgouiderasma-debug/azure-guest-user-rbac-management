GitHub Repository – Azure Guest User \& RBAC Management

Repository name:



azure-guest-user-rbac-management



Repository description:



Hands-on Azure lab demonstrating how to invite external users as Microsoft Entra ID Guest Users and assign Azure RBAC permissions at Subscription scope.

1\. Empfohlene GitHub-Struktur

So würde ich dein Repository aufbauen:



azure-guest-user-rbac-management/

│

├── README.md

│

└── screenshots/

&#x20;   ├── 01-invite-guest-user.png

&#x20;   ├── 02-guest-user-created.png

&#x20;   ├── 03-subscription-iam.png

&#x20;   ├── 04-select-rbac-role.png

&#x20;   └── 05-role-assignment-verified.png

Azure Lab: Guest User Management \& RBAC Role Assignment



1\. Project Overview



This hands-on lab demonstrates how to invite an external user to Microsoft Entra ID as a Guest User and assign Azure Role-Based Access Control (RBAC) permissions at the Subscription level.



The objective is to understand how external identities are managed in Microsoft Azure and how administrators control access to Azure resources through role-based permissions.



Technologies \& Services:



Microsoft Azure



Microsoft Entra ID



Azure Role-Based Access Control (RBAC)



Azure Subscription



Identity and Access Management (IAM)



2\. Lab Objectives



In this lab, I performed the following tasks:



Invite an external user to Microsoft Entra ID.



Create a Guest User using Microsoft Entra B2B collaboration.



Access the Azure Subscription.



Configure access permissions through Access Control (IAM).



Assign an RBAC role to the Guest User.



Verify the role assignment.



3\. Lab Environment



Component



Configuration



Cloud Platform



Microsoft Azure



Identity Provider



Microsoft Entra ID



User Type



Guest User



Resource Scope



Subscription



Access Management



Azure RBAC



Management Interface



Azure Portal



4\. Implementation – Step by Step



Step 1: Invite an External Guest User



Navigate to the Microsoft Entra Admin Center.



1.Open Microsoft Entra ID.



2.Navigate to Users.



3.Select New User.



4.Select Invite External User.



5.Enter the external user's email address.



6.Send the invitation.



The external user is invited to the organization's directory as a Guest User.







Step 2: Verify Guest User Creation



After sending the invitation, navigate to:



Microsoft Entra ID → Users



Verify that the invited user appears in the user list and has the Guest user type.





Step 3: Navigate to Subscription IAM



Open the Azure Portal.



1.Navigate to Subscriptions.



2.Select the target Subscription.



3.Open Access Control (IAM).



IAM provides centralized access management for Azure resources.





Step 3: Navigate to Subscription IAM



Open the Azure Portal.



1.Navigate to Subscriptions.



2.Select the target Subscription.



3.Open Access Control (IAM).



IAM provides centralized access management for Azure resources.





Step 4: Assign an RBAC Role



Within Access Control (IAM):



1.Select Add.



2.Select Add Role Assignment.



3.Choose the appropriate role.



4.Select the invited Guest User.



5.Review the configuration.



6.Complete the role assignment.



Example RBAC roles:



Role



Permissions



Reader



View resources but cannot modify them.



Contributor



Create, modify and delete resources.



Owner



Full resource management and permission assignment.







Step 5: Verify Role Assignment



Navigate to:



Subscription → Access Control (IAM) → Role Assignments



Verify the following:



The Guest User appears in the role assignment list.



The correct RBAC role is assigned.



The assignment scope is the intended Subscription.



5\. Technical Concepts



Microsoft Entra ID – Guest Users



Guest Users are external identities invited into an organization's Microsoft Entra ID tenant.



This enables organizations to collaborate securely with external partners, consultants and customers.



Azure RBAC



Azure Role-Based Access Control (RBAC) enables administrators to manage access to Azure resources by assigning roles to users, groups or service principals.



RBAC assignments consist of:



Security Principal: Who receives access?



Role Definition: What permissions are granted?



Scope: Where do the permissions apply?



Least Privilege Principle



Users should receive only the permissions required to perform their tasks.



Assigning Reader instead of Contributor or Owner is an example of applying the principle of least privilege when read-only access is sufficient.



6\. Key Learnings



Through this practical lab, I gained hands-on experience with:



External user management in Microsoft Entra ID.



Microsoft Entra B2B collaboration.



Azure Subscription access management.



Azure RBAC role assignments.



IAM configuration and permission verification.



Applying the principle of least privilege.



7\. Conclusion



This lab demonstrates an important aspect of Azure administration: managing external identities and controlling access to cloud resources.



Understanding Microsoft Entra ID and Azure RBAC is essential for administering secure and well-managed Azure environments.



Continuous Learning | Hands-on Practice | Azure Cloud Administration



8\. References



Microsoft Learn – What is Microsoft Entra B2B?



Microsoft Learn – Azure RBAC Overview



Microsoft Learn – Assign Azure Roles



Disclaimer: This repository documents a personal learning lab. No real customer or production environment is represented. Sensitive information such as tenant IDs, subscription IDs, email addresses and personal data should be removed from screenshots before publication.

