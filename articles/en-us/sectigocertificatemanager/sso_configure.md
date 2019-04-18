## Prerequisites

To configure Azure AD integration with Sectigo Certificate Manager, you need the following items:

- An Azure AD subscription
- A Sectigo Certificate Manager single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring Sectigo Certificate Manager for single sign-on

To configure single sign-on on **Sectigo Certificate Manager** side, you need to send the **[Downloaded Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)** and appropriate copied URLs from Azure portal to [Sectigo Certificate Manager support team](https://sectigo.com/support). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Login URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Logout URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD Identifier** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

## Additional Resources

* [How to integrate Sectigo Certificate Manager with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/sectigocertificatemanager-tutorial)
