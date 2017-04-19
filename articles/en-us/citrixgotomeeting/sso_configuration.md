 ## Prerequisites

To configure Azure AD integration with Citrix GoToMeeting, you need the following items:

- An Azure AD subscription
- A Citrix GoToMeeting single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Citrix GoToMeeting for single sign-on


1. In a different browser window, log into your [Citrix Organization Center](https://account.citrixonline.com/organization/administration/).

2. Click the **Identity Provider** tab, and then perform the following steps:  
   
	
	![SAML setup](./media/active-directory-saas-citrix-gotomeeting-tutorial/IC6892321.png "SAML setup")
   
    a. Select **Manual**

    b. In the Azure portal, on the **Configure single sign-on at Citrix GoToMeeting** dialog page, copy the  **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% value, and then paste it into the **Sign-in page URL** textbox. 

    c. In the Azure portal, on the **Configure single sign-on at Citrix GoToMeeting** dialog page, copy the **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% value, and then paste it into the **Sign-out page URL** textbox.

    d. In the Azure portal, on the **Configure single sign-on at Citrix GoToMeeting** dialog page, copy the **Azure AD SAML Entity ID** : %metadata:IssuerUri% value, and then paste it into the **Identity Provider Entity ID** textbox.

    e. To upload your downloaded certificate, click **Upload Certificate**.

    f. Click **Save**.

## Quick Reference

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

## Additional Resources

* [How to integrate Citrix GoToMeeting with Azure Active Directory](active-directory-saas-citrixgotomeeting-tutorial.md)
* [How to configure user provisioning with Citrix GoToMeeting](active-directory-saas-citrixgotomeeting-user-provisioning-tutorial.md)
