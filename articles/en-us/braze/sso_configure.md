## Prerequisites

To configure Azure AD integration with Braze, you need the following items:

- An Azure AD subscription
- A Braze single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Braze for single sign-on

To configure single sign-on on **Braze** side, you need to send the **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** and appropriate copied URLs from Azure portal to [Braze support team](mailto:support@braze.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Login URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Logout URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD Identifier** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Braze with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/braze-tutorial)
