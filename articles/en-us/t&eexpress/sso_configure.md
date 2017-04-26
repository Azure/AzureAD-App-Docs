## Prerequisites

To configure Azure AD integration with T&E Express, you need the following items:

- An Azure AD subscription
- A T&E Express single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring T&E Express for single sign-on

1. To configure single sign-on on **T&E Express** side, login to the T&E express application without SAML single sign-on using admin credentials.

2. Under the **Admin** Tab, Click on **SAML domain** to Open the SAML settings page.

	![Configure Single Sign-On](./media/tye-SAML.png)

3. Select the **Activar(Activate)** option from **No** to **SI(Yes)**. In the **Identity Provider Metadata** textbox, paste the metadata XML, which you have downloaded from Azure portal.

	![Configure Single Sign-On](./media/tyeAdmin.png)

4. Click the **Guardar(Save)** button to save the settings.	


## Quick Reference

* **Azure AD Single Sign-On Service URL**: %metadata:singleSignOnServiceUrl%

* **Azure AD SAML Entity ID**: %metadata:IssuerUri%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**


## Additional Resources

* [How to integrate T&E Express with Azure Active Directory](active-directory-saas-t&eexpress-tutorial.md)

