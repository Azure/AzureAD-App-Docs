## Prerequisites

To configure Azure AD integration with Anaplan, you need the following items:

- An Azure AD subscription
- A Anaplan single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Anaplan for single sign-on

To configure single sign-on on **Anaplan** side, you need to send the downloaded **[Metadata XML](%metadata:metadataDownloadUrl%)**, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% and **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% to [Anaplan support team](mailto:support@anaplan.com). They set this setting to have the SAML SSO connection set properly on both sides.


## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Anaplan with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-anaplan-tutorial)
