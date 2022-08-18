# Certification:  Manage Identity and Access
- Manage Azure Active Directory (Azure AD) identities 
- Manage secure access by using Azure AD 
- Manage application access 
- Manage access control Questions for this domain comprise 30% of the total questions for this exam.
# Practice Questions & Answers 

## QUESTIONS 
### 1. The following users were deleted from Azure Active Directory:

- User 1 on February 8, 2021
- User 2 on March 20, 2021
- User 3 on April 7, 2021

1. The following groups were deleted from Azure Active Directory:

- Group A on February 7, 2021
- Group B on March 20, 2021
- Group C on April 9, 2021
- Users and groups are not synced to Active Directory.

### 1. Q: On the 2nd of May 2021, you attempt to restore the deleted users and groups. Which users and groups can you restore?

### 1. Answer:
- User 3, and Group C only. 
- Users are retained for 30 days once deleted. Groups are retained for 30 days once deleted. You will be able to restore User 3 and Group C on May 2nd.

### 2. Q: What tasks can a Privileged Role Administrator perform in PIM?

### 2. Answer:
1. View request and approval history for all privileged roles. A Privileged Role Administrator can audit all approval information in PIM.
2. Enable approval for specific roles. A Privileged Role Administrator can enable approval for all PIM roles.
3. Specify users or groups to approve requests. A Privileged Role Administrator can modify all PIM components, including specifying users and groups to approve requests.

### 3. Q: In Azure AD Identity Protection when a sign-in risk is detected, what actions can IDP take to protect a user account?
### 3. Answer: 
- Require the use of multi-factor authentication (MFA)
- Requiring MFA is an appropriate response for sign-in risks.

- Block access to the web service.
- In Azure AD Identity Protection, the administrator can always choose to block or allow access to web services for user and sign-in risks.

### 4. An developer is currently developing an application that will be hosted in Azure. They require permissions to register their application and grant consent on their own behalf. The Azure AD user setting Users can register their own applications has been set to No. The Azure AD user setting Users can consent to apps accessing company data on their behalf has been set to No.

### 4. Q: Which role should you assign to the developer? The role must not grant any extra privileges.
### 3. Answer: 

1. Application Developer
- The Application Developer role grants access to register applications and grant consent on one's own behalf. Even when Users can register their own applications has been set to No and Users can consent to apps accessing company data on their behalf has been set to No.

### 5. The following permissions have been assigned to a custom role:
`     {
    "properties": {
        "roleName": "Custom Role",
        "description": "Custom Role definition",
        "assignableScopes": [
            "/subscriptions/1ecb3eac-5656-4637-9f34-8765d32ea63f"
        ],
        "permissions": [
            {
                "actions": [
                    "*/read",
                    "Microsoft.Compute/*/write"
                ],
                "notActions": [
                    "Microsoft.Storage/*/write"
                ],
                "dataActions": [],
                "notDataActions": []
            }
        ]
    }
} `
### 5. Q: When assigned to a user, will this role allow the user to create managed disks in the subscription 1ecb3eac-5656-4637-9f34-8765d32ea63f?

### 5. Answer: 
- Yes.  Managed disks are in the Microsoft.Compute provider. The user will be able to create managed disks. The notAction is not applicable to managed disks.

### 6. You have an Azure Active Directory (Azure AD) tenant named dangeroustoys.com and an Azure subscription named DTSub1. You enable Azure AD Privileged Identity Management. You need to secure the members of the Site Recovery Contributor role. The solution must ensure the administrators request access when they create labs.

### 6. Q: What should you do first?
### 6. Answer: 
- 'From Azure AD Privileged Identity Management, discover the Azure resources of DTSub1.'
- When you first set up PIM for Azure resources, you need to discover and select the resources to protect with PIM.

### 7. Q: Which AD authentication methods allow you to handle sign-in completely in the cloud as long as you are going to use only natively Azure AD-supported sign-in features?
### 7. Answer: 
- Password hash synchronization + Azure AD Seamless SSO
- Password hash synchronization + Azure Active Directory Seamless Single Sign-On (Azure AD Seamless SSO) allow you to handle sign-in completely in the cloud as long as you are going to use only natively Azure AD-supported sign-in features.

### 8. An application has been configured for your Azure AD tenant. The application requires a large number of permissions including high privilege permissions to access organization data. During a pilot deployment of the application, it was found that users were unable to provide consent during initial application access. You would like to ensure that all users in the tenant will not be required to provide consent when using the application.

### 8. Q: What action should you take?
### 8. Answer: 
- Grant tenant-wide admin consent.
- An administrator can grant consent on behalf of users in the tenant. When users access the application, they will not be required to provide consent.

### 9. Q: What built-in RBAC role allows full access to the assigned Azure resources except the ability to manage access? 
### 9. Answer: 
- Contributor:  Contributor can manage Azure resources, but not give other users rights.

### 10. Q: What is the process of a user granting authorization to an application to access protected resources on their behalf?
### 10. Answer:
- Consent: Consent occurs during the sign-in process and is the process of a user granting authorization to an application to access protected resources on their behalf.

### 11. Q: Which of the listed users can configure administrative units?
- User A is assigned the role of Global Administrator and an Azure AD Premium P1 license.
- User B is assigned the role of Security Administrator and an Azure AD Premium P2 license.
- User C is assigned the role of Privileged Role Administrator and an Azure AD Premium P1 license.
- User D is assigned the role of Global Administrator an an Azure AD Free license.
### 11. Answer: 
- User A and User C only
- The license requirements are Azure AD Premium P1 or Azure AD Premium P2. The role requirements are Global Administrator or Privileged Role Administrator. User A meets the requirements. User C meets the requirements.

### 12. Q: You create a new Azure AD group with the following properties. Which of the objects listed can you add to the group?
- Group type: Security
- Membership type: Assigned
### 12. Answer: 
1. User: Users can be added to security groups and Microsoft 365 groups.
2. Device: Devices can be added only to security groups.
3. Service principal: Service principals can only be added to security groups.

### 13. Q: What Azure CLI command is used to create a new Azure AD user?
### 13. Answer: 
- az ad user create. 
- az ad user create is the correct CLI command to create a new Azure AD user account.

### 14. Q: Which AAD authentication method allows for on-premises authentication without the need for additional infrastructure (besides agents)? The solution allows for a single point of authentication.
### 14. Answer: 
- Pass-through authentication.  Pass-through authentication (PTA) is an agent-based authentication method that allows users to sign in to both on-premises and cloud-based applications using the same passwords. Authentication occurs against local AD domain controllers. The PTA agent can be installed on any server running Windows Server 2012 R2 or later.

### 15. Q: In PIM, the process of performing one or more actions to use a role a user is eligible for is known as ____.
### 15. Answer:
- Activating the role. In PIM, the process of performing one or more actions to use a role a user is eligible for is known as activating the role.

### 16. You need to create a new group with the following properties:
- Group type: Security
- Membership type: Dynamic User
- Members: Query results in 25 Dynamic Users
- The administrator creating the group is not a member of the group. No other dynamic user groups exist in the organization.
### 16. Q: You need to purchase licenses to support the creation of this group. Your solution must also minimize costs. Which licenses should you purchase?
### 16. Answer:
- 25 Azure AD Premium P1 licenses
- One Azure AD Premium P1 license is required for each unique user that is a member of a dynamic user group. A license is not required for the administrator.
### 17. Q: You have identified that users are inviting guests and adding them to Microsoft 365 groups that have access to confidential information. You need to ensure that only members of the Global Administrator, User Administrator, and Guest Inviter roles can invite external users (guests).
- Which settings should you configure?

### 17. Answer: 
- In External Collaboration settings, configure guest invite settings.
- Guest invite settings control who can invite guests in the directory to collaborate on resources secured by Azure AD. This setting will allow you to restrict access to only members of specific admin roles.