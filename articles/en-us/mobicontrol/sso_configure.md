## Prerequisites

To configure Azure AD integration with MobiControl, you need the following items:

- An Azure AD subscription
- A MobiControl single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring MobiControl for single sign-on

To configure single sign-on on **MobiControl** side, you need to send the **App Federation Metadata Url** to [MobiControl support team](https://www.soti.net/about/contact-us/). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Login URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate MobiControl with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/mobicontrol-tutorial)
