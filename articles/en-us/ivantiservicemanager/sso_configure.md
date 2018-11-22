## Prerequisites

To configure Azure AD integration with Ivanti Service Manager, you need the following items:

- An Azure AD subscription
- An Ivanti Service Manager single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Ivanti Service Manager for single sign-on

To configure single sign-on on **Ivanti Service Manager (ISM)** side, you need to send the **[Downloaded Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**, and copied **Login URL** : %metadata:singleSignOnServiceUrl%, **Azure AD Identifier** : %metadata:IssuerUri%, **Logout URL** : %metadata:singleSignOutServiceUrl%  to [Ivanti Service Manager (ISM) support team](https://www.ivanti.com/support/contact). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

## Additional Resources

* [How to integrate Ivanti Service Manager with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/ivanti-service-manager-tutorial)
