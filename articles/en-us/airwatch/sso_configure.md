
## Overview

To enable single sign-on with AirWatch, it must be configured to use Azure Active Directory as an identity provider. This guide provides information and tips on how to perform this configuration in AirWatch.

>[!Note]: 
>This embedded guide is brand new in the new Azure portal, and we'd love to hear your thoughts. Use the Feedback ☺ button at the top of the portal to provide feedback. The older guide for using the [Azure classic portal](https://manage.windowsazure.com) to configure this application can be found [here](https://github.com/Azure/AzureAD-App-Docs/blob/master/articles/en-us/_/sso_configure.md).
 
## Prerequisites

To configure Azure AD integration with AirWatch, you need the following items:

- An Azure AD subscription
- An AirWatch single-sign on enabled subscription

> [!Note:]
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring AirWatch for single sign-on

1. In a different web browser window, log into your AirWatch company site as an administrator.

2. In the left navigation pane, click **Accounts**, and then click **Administrators**.
   
   ![Administrators](./media/active-directory-saas-airwatch-tutorial/IC791920.png "Administrators")

3. Expand the **Settings** menu, and then click **Directory Services**.
   
   ![Settings](./media/active-directory-saas-airwatch-tutorial/IC791921.png "Settings")

4. Click the **User** tab, in the **Base DN** textfield, type your domain name, and then click **Save**.
   
   ![User](./media/active-directory-saas-airwatch-tutorial/IC791922.png "User")

5. Click the **Server** tab.
   
   ![Server](./media/active-directory-saas-airwatch-tutorial/IC791923.png "Server")

6. Perform the following steps:
    
	![Upload](./media/active-directory-saas-airwatch-tutorial/IC791924.png "Upload")    
    1. As **Directory Type**, select **None**.
    2. Select **Use SAML For Authentication**.
    3. To upload the downloaded certificate, click **Upload**.

7. In the **Request** section, perform the following steps:
    
    ![Request](./media/active-directory-saas-airwatch-tutorial/IC791925.png "Request")  

    1. As **Request Binding Type**, select **POST**.
    2. In the Azure portal, on the **Configure single sign-on at Airwatch** dialog page, copy the **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% value, and then paste it into the **Identity Provider Single Sign On URL** textbox.
    3. As **NameID Format**, select **Email Address**.
    4. Click **Save**.

8. Click the **User** tab again.
    
    ![User](./media/active-directory-saas-airwatch-tutorial/IC791926.png "User")
9. In the **Attribute** section, perform the following steps:
    
    ![Attribute](./media/active-directory-saas-airwatch-tutorial/IC791927.png "Attribute")
    1. In the **Object Identifier** textbox, type **http://schemas.microsoft.com/identity/claims/objectidentifier**.
    2. In the **Username** textbox, type **http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress**.
    3. In the **Display Name** textbox, type **http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname**.
    4. In the **First Name** textbox, type **http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname**.
    5. In the **Last Name** textbox, type **http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname**.
    6. In the **Email** textbox, type **http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress**.
    7. Click **Save**.



### Next steps

To ensure users can sign-in to AirWatch after it has been configured to use Azure Active Directory, review the following tasks and topics:

- User accounts must be pre-provisioned into AirWatch prior to sign-in. To set this up, see Provisioning.
 
- Users must be assigned access to AirWatch in Azure AD to sign-in. To assign users, see Users.
 
- To configure access polices for AirWatch users, see Access Policies.
 
- For additional information on deploying single sign-on to users, see [this article](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-appssoaccess-whatis#deploying-azure-ad-integrated-applications-to-users).



## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download SAML Metdata file](%metadata:metadataDownloadUrl%)**


## Additional Resources

* [How to integrate Box with Azure Active Directory](active-directory-saas-box-tutorial.md)
* [How to configure user provisioning with Box](active-directory-saas-box-user-provisioning-tutorial.md)
