## Prerequisites

To configure Azure AD integration with Capriza Platform, you need the following items:

- An Azure AD subscription
- A Capriza Platform single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Capriza Platform for single sign-on

 To configure single sign-on on **Capriza Platform** side, you need to send the downloaded **[Certificate](%metadata:certificateDownloadBase64Url%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri% and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [Capriza Platform support team](mailTo:support@capriza.com). They set this setting to have the SAML SSO connection set properly on both sides.


## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Capriza Platform with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-capriza-tutorial)
