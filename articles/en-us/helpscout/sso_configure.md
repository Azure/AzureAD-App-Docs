## Prerequisites

To configure Azure AD integration with Help Scout, you need the following items:

- An Azure AD subscription
- A Help Scout single sign-on enabled subscription

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Help Scout for single sign-on

To configure single sign-on on the Help Scout side, upload the **[Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** downloaded from Azure portal to the Help Scout Company SAML SSO connection settings page along with the copied value of **“Azure AD Single Sign-On Service URL” : %metadata:singleSignOnServiceUrl%**. For more details on this please refer to the [Help Scout docs](http://docs.helpscout.net/article/906-enabling-sso-with-azure-ad-as-the-identity-provider) or contact [Help Scout support](help@helpscout.com). 

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Help Scout with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-helpscout-tutorial)
