## Prerequisites

To configure Azure AD integration with SAML 1.1 Token enabled LOB App, you need the following items:

- An Azure AD subscription
- A SAML 1.1 Token enabled LOB App single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring SAML 1.1 Token enabled LOB App for single sign-on

To configure single sign-on on **SAML 1.1 Token enabled LOB App** side, you need to send the **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and SAML Single Sign-On Service URL** to application support team. They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**



## Additional Resources

* [How to integrate SAML 1.1 Token enabled LOB App with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-saml-tutorial)
