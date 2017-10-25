## Prerequisites

To configure Azure AD integration with Form.com, you need the following items:

- An Azure AD subscription
- A Form.com single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Form.com for single sign-on

To configure single sign-on on **Form.com** side, you need to send the **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**, **Metadata URL**, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [Form.com support team](https://form.com/about/company/contact-us/). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**



## Additional Resources

* [How to integrate Form.com with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-formcom-tutorial)
