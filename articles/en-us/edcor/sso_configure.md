## Prerequisites

To configure Azure AD integration with Edcor, you need the following items:

- An Azure AD subscription
- A Edcor single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Edcor for single sign-on

To configure single sign-on on **Edcor** side, you need to send the **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% and **Azure AD SAML Entity ID** : %metadata:IssuerUri% to [Edcor support team](http://www.edcor.com/contact-us-2/). They set this setting to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**


## Additional Resources

* [How to integrate Edcor with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-edcor-tutorial)
