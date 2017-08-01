## Prerequisites

To configure Azure AD integration with HR2day by Merces, you need the following items:

- An Azure AD subscription
- An HR2day by Merces single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring HR2day by Merces for single sign-on

To get SSO configured for your application, contact your  [HR2day by Merces Client support team](mailTo:servicedesk@merces.nl) and attach the **[Downloaded Azure AD Signing Certificate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** file to your email. Also please do provide the **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% so that they can be configured for SSO integration.

 > [!NOTE]
 > Please mention to Merces team that this integration need Entity ID to be set with this pattern **https://hr2day.force.com/INSTANCENAME**
   
## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certificate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**



## Additional Resources

* [How to integrate HR2day by Merces with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-hr2day-tutorial)
