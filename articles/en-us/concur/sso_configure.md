## Prerequisites

To configure Azure AD integration with Concur, you need the following items:

- An Azure AD subscription
- A Concur single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Concur for single sign-on

To get SSO configured for your application, Contact [Concur Client support team](https://www.concur.co.in/contact) and provide them with the **[SAML Metadata file](%metadata:metadataDownloadUrl%)** that you can download from **Quick Reference** section.

>**Note:**
>The configuration of your Concur subscription for federated SSO via SAML is a separate task, which you must contact [Concur Client support team](https://www.concur.co.in/contact) to perform. 

## Quick Reference

* **Azure AD Single Sign-On Service URL**: %metadata:singleSignOnServiceUrl%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Concur with Azure Active Directory](active-directory-saas-concur-tutorial.md)
* [How to configure user provisioning with Concur](active-directory-saas-concur-user-provisioning-tutorial.md)
