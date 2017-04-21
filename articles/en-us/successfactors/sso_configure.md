
## Overview

To enable single sign-on with SuccessFactors, it must be configured to use Azure Active Directory as an identity provider. This guide provides information and tips on how to perform this configuration in SuccessFactors.

>[!Note]: 
>This embedded guide is brand new in the new Azure portal, and we'd love to hear your thoughts. Use the Feedback ? button at the top of the portal to provide feedback. The older guide for using the [Azure classic portal](https://manage.windowsazure.com) to configure this application can be found [here](https://github.com/Azure/AzureAD-App-Docs/blob/master/articles/en-us/_/sso_configure.md).
 
## Prerequisites

To configure Azure AD integration with SuccessFactors, you need the following items:

- An Azure AD subscription
- A SuccessFactors single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring SuccessFactors for single sign-on

1. In a different web browser window, log into your **SuccessFactors admin portal** as an administrator.
	
2. Visit **Application Security** and native to **Single Sign On Feature**. 

3. Place any value in the **Reset Token** and click **Save Token** to enable SAML SSO.
      
	![Configuring single sign-on on app side](./media/active-directory-saas-successfactors-tutorial/tutorial_successfactors_07.png) 

    > [!NOTE] 
    > This value is just used as the on/off switch. If any value is saved, the SAML SSO is ON. If a blank value is saved the SAML SSO is OFF.

4. Native to below screenshot and perform the following actions.
   
    ![Configuring single sign-on on app side](./media/active-directory-saas-successfactors-tutorial/tutorial_successfactors_08.png)
   
    a. Select the **SAML v2 SSO** Radio Button
   
    b. Set the SAML Asserting Party Name(e.g. SAml issuer + company name).
   
    c. In the **Issuer URL** textbox, paste the **SAML Entity ID** value you have copied from the **Configure sign-on** window of the Azure portal..
   
    d. Select **Response(Customer Generated/IdP/AP)** as **Require Mandatory Signature**.
   
    e. Select **Enabled** as **Enable SAML Flag**.
   
    f. Select **No** as **Login Request Signature(SF Generated/SP/RP)**.
   
    g. Select **Browser/Post Profile** as **SAML Profile**.
   
    h. Select **No** as **Enforce Certificate Valid Period**.
   
    i. Copy the content of the downloaded certificate file, and then paste it into the **SAML Verifying Certificate** textbox.

    > [!NOTE] 
    > The certificate content must have begin certificate and end certificate tags.

5. Navigate to SAML V2, and then perform the following steps:
   
    ![Configuring single sign-on on app side](./media/active-directory-saas-successfactors-tutorial/tutorial_successfactors_09.png)
   
    a. Select **Yes** as **Support SP-initiated Global Logout**.
   
    b. In the **Global Logout Service URL (LogoutRequest destination)** textbox put the value of **Sign-Out URL** from Azure AD application configuration wizard.
   
    c. Select **No** as **Require sp must encrypt all NameID element**.
   
    d. Select **unspecified** as **NameID Format**.
   
    e. Select **Yes** as **Enable sp initiated login (AuthnRequest)**.
   
    f. In the **Send request as Company-Wide issuer** textbox put the value of **Configure sign-on** from Azure AD application configuration wizard.
6. Perform these steps if you want to make the login usernames Case Insensitive, .
   
	a. Visit **Company Settings**(near the bottom).
   
	b. select checkbox near **Enable Non-Case-Sensitive Username**.
   
	c.Click **Save**.
   
	![Configuring single sign-on on app side](./media/active-directory-saas-successfactors-tutorial/tutorial_successfactors_10.png)

    > [!NOTE] 
    > If you try to enable this, the system checks if it will create a duplicate SAML login name. For example if the customer has usernames User1 and user1. Taking away case sensitivity makes these duplicates. The system will give you an error message and will not enable the feature. The customer will need to change one of the usernames so it’s actually spelled different. 


### Next steps

To ensure users can sign-in to SuccessFactors after it has been configured to use Azure Active Directory, review the following tasks and topics:

- User accounts must be pre-provisioned into SuccessFactors prior to sign-in. To set this up, see Provisioning.
 
- Users must be assigned access to SuccessFactors in Azure AD to sign-in. To assign users, see Users.
 
- To configure access polices for SuccessFactors users, see Access Policies.
 
- For additional information on deploying single sign-on to users, see [this article](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-appssoaccess-whatis#deploying-azure-ad-integrated-applications-to-users).



## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SMAL Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**


