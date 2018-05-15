## Prerequisites

To configure Azure AD integration with FiscalNote, you need the following items:

- An Azure AD subscription
- A FiscalNote single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring FiscalNote for single sign-on

To configure single sign-on on **FiscalNote** side, you need to send the downloaded **[Certificate(Raw)](%metadata:CertificateDownloadRawUrl%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [FiscalNote support team](mailto:support@fiscalnote.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

## Additional Resources

* [How to integrate FiscalNote with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-fiscalnote-tutorial)
