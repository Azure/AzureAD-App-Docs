## Prerequisites

To configure Azure AD integration with Tidemark, you need the following items:

- An Azure AD subscription
- A Tidemark single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Tidemark for single sign-on

 To configure single sign-on on **Tidemark** side, you need to send the downloaded **[Certificate(Base64)](%metadata:certificateDownloadBase64Url%)**, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [Tidemark support team](http://www.tidemark.com/contact-us). They set this setting to have the SAML SSO connection set properly on both sides.


## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**



## Additional Resources

* [How to integrate Tidemark with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-tidemark-tutorial)
