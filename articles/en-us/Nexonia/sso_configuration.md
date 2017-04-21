## Prerequisites

To configure Azure AD integration with Nexonia, you need the following items:

- An Azure AD subscription
- A Nexonia single-sign on enabled subscription

> [!Note]:
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Nexonia for single sign-on

1. To get SSO configured for your application, contact [Nexonia support team](http://www.nexonia.com/contact-us/) and provide them with the following:

	• The downloaded **[Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

	• The **Azure AD SAML Entity ID** : %metadata:IssuerUri%

	• The **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

	• The **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%





## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**



## Additional Resources

* [How to integrate Box with Azure Active Directory](active-directory-saas-box-tutorial.md)
* [How to configure user provisioning with Box](active-directory-saas-box-user-provisioning-tutorial.md)
