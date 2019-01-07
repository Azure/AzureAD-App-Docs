## Prerequisites

To configure Azure AD integration with Workable, you need the following items:

- An Azure AD subscription
- A Workable single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Workable for single sign-on

To enable SSO in Workable, contact your dedicated Workable account manager and provide them with the following items.

1. Login URL : %metadata:singleSignOnServiceUrl%

2. [Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)

3. Logout URL : %metadata:singleSignOutServiceUrl%

Once Single Sign On has been enabled, your Workable account manager will let you know and you can use [Workable's SSO page](https://www.workable.com/sso/signin) to login using your Workable account subdomain.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Workable with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/workable-tutorial)
