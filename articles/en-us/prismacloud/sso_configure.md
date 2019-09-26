## Prerequisites

To configure Azure AD integration with Prisma Cloud, you need the following items:

- An Azure AD subscription
- A Prisma Cloud single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring Prisma Cloud for single sign-on

To configure single sign-on on **Prisma Cloud** side, you need to send the downloaded **Certificate (Base64)** and appropriate copied URLs from Azure portal to [Prisma Cloud support team](mailto:support@paloaltonetworks.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Login URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Prisma Cloud with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/prisma-cloud-tutorial)
