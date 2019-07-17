## Prerequisites

To configure Azure AD integration with JFrog Artifactory, you need the following items:

- An Azure AD subscription
- A JFrog Artifactory single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring JFrog Artifactory for single sign-on

To configure single sign-on on **JFrog Artifactory** side, you need to send the downloaded **Certificate (Raw)** and appropriate copied URLs from Azure portal to [JFrog Artifactory support team](https://support.jfrog.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Login URL** : %metadata:singleSignOnServiceUrl%

* **Logout URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD Identifier** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate JFrog Artifactory with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/jfrog-artifactory-tutorial)
