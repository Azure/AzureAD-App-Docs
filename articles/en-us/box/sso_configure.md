
## Overview

To enable single sign-on with Box, it must be configured to use Azure Active Directory as an identity provider. This guide provides information and tips on how to perform this configuration in Box.

>[!Note]: 
>This embedded guide is brand new in the new Azure portal, and we'd love to hear your thoughts. Use the Feedback ? button at the top of the portal to provide feedback. The older guide for using the [Azure classic portal](https://manage.windowsazure.com) to configure this application can be found [here](https://github.com/Azure/AzureAD-App-Docs/blob/master/articles/en-us/_/sso_configure.md).
 
## Prerequisites

To configure Azure AD integration with Box, you need the following items:

- An Azure AD subscription
- A Box single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Box for single sign-on


To get SSO configured for your application, Contact [Box Client support team](https://community.box.com/t5/Community/ct-p/English) and provide them with the **SAML Metadata XML** file which you can download from **Quick Reference** section.



### Next steps

To ensure users can sign-in to Box after it has been configured to use Azure Active Directory, review the following tasks and topics:

- User accounts must be pre-provisioned into Box prior to sign-in. To set this up, see Provisioning.
 
- Users must be assigned access to Box in Azure AD to sign-in. To assign users, see Users.
 
- To configure access polices for Box users, see Access Policies.
 
- For additional information on deploying single sign-on to users, see [this article](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-appssoaccess-whatis#deploying-azure-ad-integrated-applications-to-users).



## Quick Reference

* **[Download SAML Metdata file](%metadata:metadataDownloadUrl%)**

## Additional resources

* [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](active-directory-saas-tutorial-list.md)
* [What is application access and single sign-on with Azure Active Directory?](active-directory-appssoaccess-whatis.md)
