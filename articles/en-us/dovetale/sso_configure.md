## Prerequisites

To configure Azure AD integration with Dovetale, you need the following items:

- An Azure AD subscription
- A Dovetale single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Dovetale for single sign-on

To configure single sign-on on **Dovetale** side, you need to send the **App Federation Metadata Url, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%** to [Dovetale support team](mailto:support@dovetale.com). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

## Additional Resources

* [How to integrate Dovetale with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/dovetale-tutorial)
