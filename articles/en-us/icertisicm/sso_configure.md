## Prerequisites

To configure Azure AD integration with Icertis Contract Management Platform, you need the following items:

- An Azure AD subscription
- A Icertis Contract Management Platform single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Icertis Contract Management Platform for single sign-on

To configure single sign-on on **Icertis Contract Management Platform** side, you need to send the **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)** and **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [Icertis Contract Management Platform support team](https://www.icertis.com/company/contact/).

## Quick Reference

* **Azure AD Single Sign-On Service URL** : `https://login.microsoftonline.com/_my_directory_id_/wsfed`

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Icertis Contract Management Platform with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-icertisicm-tutorial)
