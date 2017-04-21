
## Overview

To enable single sign-on with atlassiancloud, it must be configured to use Azure Active Directory as an identity provider. This guide provides information and tips on how to perform this configuration in atlassiancloud.

>[!Note]: 
>This embedded guide is brand new in the new Azure portal, and we'd love to hear your thoughts. Use the Feedback ? button at the top of the portal to provide feedback. The older guide for using the [Azure classic portal](https://manage.windowsazure.com) to configure this application can be found [here](https://github.com/Azure/AzureAD-App-Docs/blob/master/articles/en-us/_/sso_configure.md).
 
## Prerequisites

To configure Azure AD integration with atlassiancloud, you need the following items:

- An Azure AD subscription
- A atlassiancloud single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring atlassiancloud for single sign-on

1. To get SSO configured for your application, login to the Atlassian Portal using the administrator rights.

2. In the Authentication section of the left navigation click **Domains**.

	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_06.png)

    a. In the textbox, type your domain name, and then click **Add domain**.
		
	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_07.png)

    b. To verify the domain, click **Verify**. 

	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_08.png)

    c. Download the domain verification html file, upload it to the root folder of  your domain's website, and then click **Verify domain**.
	
	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_09.png)

    d. Once the domain is verified, the value of the **Stauts** field is **Verified**.

	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_10.png)

3. In the left navigation bar, click **SAML**.
 
	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_11.png)

4. Create a new SAML Configuration and add the Identity provider configuration.

	a. Paste the Entity Id in the Identity Provider Entity ID field.

	b. Paste the SAML SSO URL in the Identity Provider SSO URL box.

	c. Open the downloaded certificate from Azure AD and copy the values without the Begin and End lines and paste it in the Public X509 certificate box.

	d. Save the settings.

	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_12.png)
 
5. Update the Azure AD settings to make sure that you have setup the correct Identifier URL.

	a. Copy the SP Identity ID from the SAML screen and paste it in Azure AD as the **Identifier** value.
  
	b. Sign On URL is the tenant URL of your Atlassian Cloud.

	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_atlassiancloud_13.png)
	
6. In the Azure Portal, Click **Save** button.

	![Configure Single Sign-On](./media/active-directory-saas-atlassiancloud-tutorial/tutorial_general_400.png)

### Next steps

To ensure users can sign-in to atlassiancloud after it has been configured to use Azure Active Directory, review the following tasks and topics:

- User accounts must be pre-provisioned into atlassiancloud prior to sign-in. To set this up, see Provisioning.
 
- Users must be assigned access to atlassiancloud in Azure AD to sign-in. To assign users, see Users.
 
- To configure access polices for atlassiancloud users, see Access Policies.
 
- For additional information on deploying single sign-on to users, see [this article](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-appssoaccess-whatis#deploying-azure-ad-integrated-applications-to-users).

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD SMAL Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**


