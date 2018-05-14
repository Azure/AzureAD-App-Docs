## Prerequisites

To configure Azure AD integration with Arc Publishing - SSO, you need the following items:

- An Azure AD subscription
- An Arc Publishing - SSO single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Arc Publishing - SSO for single sign-on

To configure single sign-on on **Arc Publishing - SSO** side, you need to send the **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**, Sign-Out URL, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [Arc Publishing - SSO support team](mailto:inf@washpost.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Arc Publishing - SSO with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-arc-tutorial)
