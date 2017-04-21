
## Overview

To enable single sign-on with ADP Globalview, it must be configured to use Azure Active Directory as an identity provider. This guide provides information and tips on how to perform this configuration in ADP Globalview.

>[!Note]: 
>This embedded guide is brand new in the new Azure portal, and we'd love to hear your thoughts. Use the Feedback ☺ button at the top of the portal to provide feedback. The older guide for using the [Azure classic portal](https://manage.windowsazure.com) to configure this application can be found [here](https://github.com/Azure/AzureAD-App-Docs/blob/master/articles/en-us/_/sso_configure.md).
 
## Prerequisites

To configure Azure AD integration with ADP Globalview, you need the following items:

- An Azure AD subscription
- An ADP Globalview single-sign on enabled subscription

> [!Note]:
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring ADP Globalview for single sign-on

10. To configure single sign-on on **ADP Globalview** side, you need to send the downloaded **certificate (Base64)**,**Sign-Out URL, SAML Entity ID and SAML Single Sign-On Service URL** to [ADP Globalview support](https://www.adp.com/contact-us/overview.aspx). They will set this up in order to have the SAML SSO connection set properly on both sides.


### Next steps

To ensure users can sign-in to ADP Globalview after it has been configured to use Azure Active Directory, review the following tasks and topics:

- User accounts must be pre-provisioned into ADP Globalview prior to sign-in. To set this up, see Provisioning.
 
- Users must be assigned access to ADP Globalview in Azure AD to sign-in. To assign users, see Users.
 
- To configure access polices for ADP Globalview users, see Access Policies.
 
- For additional information on deploying single sign-on to users, see [this article](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-appssoaccess-whatis#deploying-azure-ad-integrated-applications-to-users).



## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**


## Additional Resources

* [How to integrate Box with Azure Active Directory](active-directory-saas-box-tutorial.md)
* [How to configure user provisioning with Box](active-directory-saas-box-user-provisioning-tutorial.md)
