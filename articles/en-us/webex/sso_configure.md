
## Overview

To enable single sign-on with Cisco WebEx, it must be configured to use Azure Active Directory as an identity provider. This guide provides information and tips on how to perform this configuration in Cisco WebEx.

>[!Note]: 
>This embedded guide is brand new in the new Azure portal, and we'd love to hear your thoughts. Use the Feedback ? button at the top of the portal to provide feedback. The older guide for using the [Azure classic portal](https://manage.windowsazure.com) to configure this application can be found [here](https://github.com/Azure/AzureAD-App-Docs/blob/master/articles/en-us/_/sso_configure.md).
 
## Prerequisites

To configure Azure AD integration with Cisco WebEx, you need the following items:

- An Azure AD subscription
- A Cisco WebEx single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Cisco WebEx for single sign-on

1. To configure single sign-on on **Cisco Webex** side, you need to send the downloaded **Metadata XML** and **SAML Entity ID** to [Cisco Webex Client support team](https://www.webex.co.in). They will set this up in order to have the SAML SSO connection set properly on both sides.

2. In a different web browser window, log into your Cisco Webex company site as an administrator.

3. In the menu on the top, click **Site Administration**.

	![Site Administration](./media\active-directory-saas-ciscowebex-tutorial/IC777621.png "Site Administration")

4. In the **Manage Site** section, click **SSO Configuration**.
   
	![SSO Configuration](./media\active-directory-saas-ciscowebex-tutorial/IC777622.png "SSO Configuration")

5. In the Federated Web SSO Configuration section, perform the following steps:
   
	![Federated SSO Configuration](./media\active-directory-saas-ciscowebex-tutorial/IC777623.png "Federated SSO Configuration")  

	a. From the **Federation Protocol** list, select **SAML 2.0**.

	b. Create a **Base-64 encoded** file from your downloaded certificate.
  
    >[!TIP]
    >For more details, see [How to convert a binary certificate into a text file](http://youtu.be/PlgrzUZ-Y1o)
    
	c. Open your base-64 encoded certificate in notepad, and then copy the content of it.

	d. Click **Import SAML Metadata**, and then paste your base-64 encoded certificate.

	e. In the Azure classic portal, on the **Configure single sign-on at Cisco Webex** dialog page, copy the **SAML Entity ID** value, and then paste it into the **Issuer for SAML (IdP ID)** textbox.

	f. In the Azure classic portal, on the **Configure single sign-on at Cisco Webex** dialog page, copy the **SAML Single Sign-On Service URL** value, and then paste it into the **Customer SSO Service Login URL** textbox.

	g. From the **NameID Format** list, select **Email address**.

	h. In the **AuthnContextClassRef** textbox, type **urn:oasis:names:tc:SAML:2.0:ac:classes:Password**.

	i. In the Azure classic portal, on the **Configure single sign-on at Cisco Webex** dialog page, copy the **Sign-Out URL** value, and then paste it into the **Customer SSO Service Logout URL** textbox.
   
	j. Click **Update**.


### Next steps

To ensure users can sign-in to Cisco WebEx after it has been configured to use Azure Active Directory, review the following tasks and topics:

- User accounts must be pre-provisioned into Cisco WebEx prior to sign-in. To set this up, see Provisioning.
 
- Users must be assigned access to Cisco WebEx in Azure AD to sign-in. To assign users, see Users.
 
- To configure access polices for Cisco WebEx users, see Access Policies.
 
- For additional information on deploying single sign-on to users, see [this article](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-appssoaccess-whatis#deploying-azure-ad-integrated-applications-to-users).



## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SMAL Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metdata file](%metadata:metadataDownloadUrl%)**


