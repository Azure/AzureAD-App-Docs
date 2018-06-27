## Prerequisites

To configure Azure AD integration with Certain Admin SSO, you need the following items:

- An Azure AD subscription
- A Certain Admin SSO single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Certain Admin SSO for single sign-on

To configure single sign-on on **Certain Admin SSO** side, you need to send the **[Downloaded Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%** to [Certain Admin SSO support team](mailto:integrations@certain.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

## Additional Resources

* [How to integrate Certain Admin SSO with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/certainadminsso-tutorial)
