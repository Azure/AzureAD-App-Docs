## Prerequisites

To configure Azure AD integration with Certent Equity Management, you need the following items:

- An Azure AD subscription
- A Certent Equity Management single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Certent Equity Management for single sign-on

To configure single sign-on on **Certent Equity Management** side, you need to send the **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)** and appropriate copied URLs from Azure portal to Certent Integration Analyst assigned by Customer Success Manager. They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Login URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Logout URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD Idenifier** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Certent Equity Management with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/certent-equity-management-tutorial)
