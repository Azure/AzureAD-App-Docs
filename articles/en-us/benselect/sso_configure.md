## Prerequisites

To configure Azure AD integration with BenSelect, you need the following items:

- An Azure AD subscription
- A BenSelect single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring BenSelect for single sign-on

To configure single sign-on on **BenSelect** side, you need to send the downloaded **Certificate(Raw)** and **Sign-Out URL**, **Azure AD SAML Entity ID** : %metadata:IssuerUri%, and **SAML Single Sign-On Service URL** to [BenSelect support team](mailto:support@selerix.com).

   >[!NOTE]
   >You need to mention that this integration requires the SHA256 algorithm (SHA1 is not supported) to set the SSO on the appropriate server like app2101 etc. 

## Quick Reference

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

## Additional Resources

* [How to integrate BenSelect with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-benselect-tutorial)
