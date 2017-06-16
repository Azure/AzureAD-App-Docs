## Prerequisites

To configure Azure AD integration with BeeLine, you need the following items:

- An Azure AD subscription
- A BeeLine single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring BeeLine for single sign-on

To configure single sign-on on **BeeLine** side, you need to send the **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)** and **Azure AD SAML Entity ID** : %metadata:IssuerUri%, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% to [BeeLine support team](https://www.beeline.com/contact-us/).

## Quick Reference

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate BeeLine with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-beeline-tutorial)
