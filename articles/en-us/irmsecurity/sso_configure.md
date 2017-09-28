## Prerequisites

To configure Azure AD integration with Synergi, you need the following items:

- An Azure AD subscription
- A Synergi single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Synergi for single sign-on

To configure single sign-on on **Synergi** side, you need to send the **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, and **Azure AD SAML Entity ID** : %metadata:IssuerUri% to [Synergi support team](https://www.irmsecurity.com/contact/).

## Quick Reference

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Synergi with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-synergi-tutorial)
