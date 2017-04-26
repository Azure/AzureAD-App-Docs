## Prerequisites

To configure Azure AD integration with ADP Globalview, you need the following items:

- An Azure AD subscription
- An ADP Globalview single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring ADP Globalview for single sign-on

1. To configure single sign-on on **ADP Globalview** side, you need to send the downloaded **[certificate(Base64)](%metadata:certificateDownloadBase64Url%)**, **Azure AD Sign Out URL**: %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID**: %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL**: %metadata:singleSignOnServiceUrl% to [ADP Globalview support](https://www.adp.com/contact-us/overview.aspx). They set up to have the SAML SSO connection set properly on both sides.

## Quick Reference

* **Azure AD Single Sign-On Service URL**: %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL**: %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID**: %metadata:IssuerUri%

* **[Download Azure AD Signing Certificate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

 
## Additional Resources

* [How to integrate Absorb ADP Globalview with Azure Active Directory](active-directory-saas-adpglobalview-tutorial.md)
