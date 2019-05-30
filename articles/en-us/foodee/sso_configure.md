## Prerequisites

To configure Azure AD integration with Foodee, you need the following items:

- An Azure AD subscription
- A Foodee single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring Foodee for single sign-on

1. In a different web browser window, sign in to Foodee as an Administrator.

2. Click on **profile logo** on the top right corner of the page then navigate to **Single Sign On** and perform the following steps:

	 ![Foodee configuration](./media/config01.png)

	a. In the **IDP NAME** text box, type the name like ex:Azure.

	b. Open the **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)** in Notepad, copy its content and paste it in the **IDP METADATA XML** text box.

	c. Click **Save**.

## Quick Reference

* **Azure AD Login URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Foodee with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/foodee-tutorial)
