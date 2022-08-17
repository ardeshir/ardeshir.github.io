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
- User 3, and Group C only
 1. Users are retained for 30 days once deleted. Groups are retained for 30 days once deleted. You will be able to restore User 3 and Group C on May 2nd.

### 2. Q: What tasks can a Privileged Role Administrator perform in PIM?

### 2. Answer:

1. View request and approval history for all privileged roles.
- A Privileged Role Administrator can audit all approval information in PIM.

2. Enable approval for specific roles.
- A Privileged Role Administrator can enable approval for all PIM roles.

3. Specify users or groups to approve requests.
- A Privileged Role Administrator can modify all PIM components, including specifying users and groups to approve requests.

### 3. Q: In Azure AD Identity Protection when a sign-in risk is detected, what actions can IDP take to protect a user account?
### 3. Answer: 
1. Require the use of multi-factor authentication (MFA)
- Requiring MFA is an appropriate response for sign-in risks.

2. Block access to the web service.
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
1. Yes
- Managed disks are in the Microsoft.Compute provider. The user will be able to create managed disks. The notAction is not applicable to managed disks.

### 6. You have an Azure Active Directory (Azure AD) tenant named dangeroustoys.com and an Azure subscription named DTSub1. You enable Azure AD Privileged Identity Management. You need to secure the members of the Site Recovery Contributor role. The solution must ensure the administrators request access when they create labs.

### 6. Q: What should you do first?
### 6. Answer: 
1. 'From Azure AD Privileged Identity Management, discover the Azure resources of DTSub1.'
- When you first set up PIM for Azure resources, you need to discover and select the resources to protect with PIM.

### 7. Q: Which AD authentication methods allow you to handle sign-in completely in the cloud as long as you are going to use only natively Azure AD-supported sign-in features?
### 7. Answer: 
1. Password hash synchronization + Azure AD Seamless SSO
- Password hash synchronization + Azure Active Directory Seamless Single Sign-On (Azure AD Seamless SSO) allow you to handle sign-in completely in the cloud as long as you are going to use only natively Azure AD-supported sign-in features.