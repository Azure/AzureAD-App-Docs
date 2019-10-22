## Prerequisites

To configure Azure AD integration with Contentful, you need the following items:

- An Azure AD subscription
- A Contentful single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring Contentful for single sign-on

Follow these steps to configure single sign-on on **Contentful** side.

1. In [Contentful](https://app.contentful.com), navigate to the SSO setup page in Organization Settings.
1. Click on **Set up SSO**.
1. Copy and paste the Login URL from the **Set up Contentful** section in Azure AD.
1. Copy and paste the **[Certifcate](%metadata:CertificateDownloadRawUrl%)** from the Base64 certificate file you downloaded from Azure AD.
1. Set up an SSO name for SP-initiated login.
1. Click on **Enable SSO**.

If that doesn't work, reach out to [Contentful support team](mailto:support@contentful.com).

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Contentful with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/contentful-tutorial)
