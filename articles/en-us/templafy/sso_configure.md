## Prerequisites

To configure Azure AD integration with Templafy, you need the following items:

- An Azure AD subscription
- A Templafy single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Templafy for single sign-on

To configure single sign-on on **Templafy** side, you need to send the **App Federation Metadata Url** to [Templafy support team](mailto:support@templafy.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Login URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Templafy with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/templafy-tutorial)
