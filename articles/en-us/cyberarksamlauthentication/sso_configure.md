## Prerequisites

To configure Azure AD integration with CyberArk SAML Authentication, you need the following items:

- An Azure AD subscription
- A CyberArk SAML Authentication single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring CyberArk SAML Authentication for single sign-on

To configure single sign-on on **CyberArk SAML Authentication** side, you need to send the downloaded **Certificate (Raw)** and appropriate copied URLs from Azure portal to [CyberArk SAML Authentication support team](mailto:bizdevtech@cyberark.com). They set this setting to have the SAML SSO connection set properly on both sides

## Quick Reference

* **Login URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate CyberArk SAML Authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/cyberark-saml-authentication-tutorial)
