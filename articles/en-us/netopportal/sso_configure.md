## Prerequisites

To configure Azure AD integration with Netop Portal, you need the following items:

- An Azure AD subscription
- A Netop Portal single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Netop Portal for single sign-on

To configure single sign-on on **Netop Portal** side, you need to send the **[Downloaded Federation Metadata XML](%metadata:metadataDownloadUrl%)** and appropriate copied URLs from Azure portal to [Netop Portal support team](mailto:casemanager@netop.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download Federation Metadata XML](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Netop Portal with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/netop-portal-tutorial)
