## Prerequisites

To configure Azure AD integration with Soonr Workplace, you need the following items:

- An Azure AD subscription
- A Soonr Workplace single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial here: [Trial offer](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Soonr Workplace for single sign-on

To configure single sign-on on **Soonr Workplace** side, you need to send the **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)**, **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% to [Soonr Workplace support team](https://awp.autotask.net/help/). They set this setting to have the SAML SSO connection set properly on both sides.

   >[!NOTE]
   >This application is superseded by <a href="https://azure.microsoft.com/en-us/marketplace/partners/autotask-corporataion/autotask/">Autotask Workplace</a> and you can refer <a href="https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-autotaskworkplace-tutorial">this</a> tutorial for configuring the application with Azure AD.


## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Soonr Workplace with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-soonr-tutorial)
