## Prerequisites

To configure Azure AD integration with JOBHUB, you need the following items:

- An Azure AD subscription
- A JOBHUB single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring JOBHUB for single sign-on

To configure single sign-on on **JOBHUB** side, you need to send the **Thumbprint value** and appropriate copied URLs from Azure portal to [JOBHUB support team](mailto:platform@pasonagroup.co.jp). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Login URL** : %metadata:singleSignOnServiceUrl%

* **Logout URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD Identifier** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate JOBHUB with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/jobhub-tutorial)
