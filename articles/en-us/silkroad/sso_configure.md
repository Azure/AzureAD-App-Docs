## Prerequisites

To configure Azure AD integration with SilkRoad Life Suite, you need the following items:

- An Azure AD subscription
- A SilkRoad Life Suite single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring SilkRoad Life Suite for single sign-on

1. Sign-on to your SilkRoad company site as administrator. 
 
    >[!NOTE] 
    > To obtain access to the SilkRoad Life Suite Authentication application for configuring federation with Microsoft Azure AD, please contact SilkRoad Support or your SilkRoad Services representative.

2. Go to **Service Provider**, and then click **Federation Details**. 
   
    ![Azure AD Single Sign-On][10]

3. Click **Download Federation Metadata**, and then save the metadata file on your computer.
   
    ![Azure AD Single Sign-On][11] 

4. In your **SilkRoad** application, click **Authentication Sources**.
   
    ![Azure AD Single Sign-On][12] 

5. Click **Add Authentication Source**. 
   
    ![Azure AD Single Sign-On][13] 

6. In the **Add Authentication Source** section, perform the following steps: 
   
    ![Azure AD Single Sign-On][14]
  
    a. Under **Option 2 - Metadata File**, click **Browse** to upload the downloaded metadata file from Azure portal.
  
    b. Click **Create Identity Provider using File Data**.

7. In the **Authentication Sources** section, click **Edit**. 
    
     ![Azure AD Single Sign-On][15] 

8. On the **Edit Authentication Source** dialog, perform the following steps: 
    
     ![Azure AD Single Sign-On][16] 

    a. As **Enabled**, select **Yes**.

	b. In the **EntityId** textbox, paste the value of **SAML Entity ID** which you have copied from Azure portal.
   
    c. In the **IdP Description** textbox, type a description for your configuration (for example: *Azure AD SSO*).

	d. In the **Metadata File** textbox, Upload the **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)** file from Azure portal.
  
    e. In the **IdP Name** textbox, type a name that is specific to your configuration (for example: *Azure SP*).
  
	f. In the **Logout Service URL** textbox, paste the value of **Sign-Out URL** which you have copied from Azure portal.

	g. In the **sign-on service URL** textbox, paste the value of **SAML Single Sign-On Service URL** which you have copied from Azure portal.

    h. Click **Save**.

9. Disable all other authentication sources. 
    
     ![Azure AD Single Sign-On][17]

## Quick Reference

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate SilkRoad Life Suite with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-silkroad-life-suite-tutorial)

<!--Image references-->

[10]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_06.png
[11]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_07.png
[12]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_08.png
[13]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_09.png
[14]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_10.png
[15]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_11.png
[16]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_12.png
[17]: ./media/active-directory-saas-silkroad-life-suite-tutorial/tutorial_silkroad_13.png