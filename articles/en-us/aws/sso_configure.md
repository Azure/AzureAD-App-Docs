## Prerequisites

To configure Azure AD integration with Amazon Web Services (AWS), you need the following items:

- An Azure AD subscription
- A Amazon Web Services (AWS) single-sign on enabled subscription

> [!Note]:
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Amazon Web Services (AWS) for single sign-on

1. In a different browser window, sign-on to your Amazon Web Services (AWS) company site as administrator.

2. Click **Console Home**.
   
    ![Configure Single Sign-On][11]

3. Click **Identity and Access Management**. 
   
    ![Configure Single Sign-On][12]

4. Click **Identity Providers**, and then click **Create Provider**. 
   
    ![Configure Single Sign-On][13]

5. On the **Configure Provider** dialog page, perform the following steps: 
   
    ![Configure Single Sign-On][14]
 
  	a. As **Provider Type**, select **SAML**.

  	b. In the **Provider Name** textbox, type a provider name (e.g.: *WAAD*).

  	c. To upload your downloaded metadata file (**[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**), click **Choose File**.

  	d. Click **Next Step**.

6. On the **Verify Provider Information** dialog page, click **Create**. 
    
    ![Configure Single Sign-On][15]

7. Click **Roles**, and then click **Create New Role**. 
    
    ![Configure Single Sign-On][16]

8. On the **Set Role Name** dialog, perform the following steps: 
    
    ![Configure Single Sign-On][17] 

  	a. In the **Role Name** textbox, type a role name (e.g.: *TestUser*). 

  	b. Click **Next Step**.

9. On the **Select Role Type** dialog, perform the following steps: 
    
    ![Configure Single Sign-On][18] 

  	a. Select **Role For Identity Provider Access**. 

  	b. In the **Grant Web Single Sign-On (WebSSO) access to SAML providers** section, click **Select**.

10. On the **Establish Trust** dialog, perform the following steps:  
    
    ![Configure Single Sign-On][19] 

  	a. As SAML provider, select the SAML provider you have created previousley (e.g.: *WAAD*) 
  
  	b. Click **Next Step**.

11. On the **Verify Role Trust** dialog, click **Next Step**. 
    
    ![Configure Single Sign-On][32]

12. On the **Attach Policy** dialog, click **Next Step**.  
    
    ![Configure Single Sign-On][33]

13. On the **Review** dialog, perform the following steps:   
    
    ![Configure Single Sign-On][34] 

  	a. Copy the **Role ARN** value.  

  	b. Copy the **Trusted Entities** ARN value.
 
  	c. Click **Create Role**.
 

## Quick Reference

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Amazon Web Services (AWS) with Azure Active Directory](active-directory-saas-amazonwebservices(aws)-tutorial.md)

[11]: ./media/ic795031.png
[12]: ./media/ic795032.png
[13]: ./media/ic795033.png
[14]: ./media/ic795034.png
[15]: ./media/ic795035.png
[16]: ./media/ic795022.png
[17]: ./media/ic795023.png
[18]: ./media/ic795024.png
[19]: ./media/ic795025.png
[32]: ./media/ic7950251.png
[33]: ./media/ic7950252.png
[34]: ./media/ic7950253.png