## Prerequisites

To configure Azure AD integration with NEOGOV, you need the following items:

- An Azure AD subscription
- A NEOGOV single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring NEOGOV for single sign-on

To configure single sign-on on **NEOGOV** side, you need to send the **App Federation Metadata Url** to [NEOGOV support team](mailto:itops@neogov.net). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Login URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate NEOGOV with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/neogov-tutorial)
