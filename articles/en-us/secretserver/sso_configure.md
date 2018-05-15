## Prerequisites

To configure Azure AD integration with Secret Server (On-Premises), you need the following items:

- An Azure AD subscription
- A Secret Server (On-Premises) single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Secret Server (On-Premises) for single sign-on

To configure single sign-on on **Secret Server (On-Premises)** side, you need to send the downloaded **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%, and **Azure AD SAML Entity ID** : %metadata:IssuerUri% to [Secret Server (On-Premises) support team](https://thycotic.force.com/support/s/). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Secret Server (On-Premises) with Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-secretserver-on-premises-tutorial)
