## Prerequisites

To configure Azure AD integration with IQNavigator VMS, you need the following items:

- An Azure AD subscription
- A IQNavigator VMS single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring IQNavigator VMS for single sign-on

To configure single sign-on on **IQNavigator VMS** side, you need to send the **Metadata URL**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [IQNavigator VMS support team](https://www.beeline.com/iqn-product-support/). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

## Additional Resources

* [How to integrate IQNavigator VMS with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-iqnavigatorvms-tutorial)
