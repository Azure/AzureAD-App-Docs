## Prerequisites

To configure Azure AD integration with Halogen Software, you need the following items:

- An Azure AD subscription
- A Halogen Software single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Halogen Software for single sign-on

1. In a different browser window, sign-on to your **Halogen Software** application as an administrator.

2. Click the **Options** tab. 
   
    ![What is Azure AD Connect][12]

3. In the left navigation pane, click **SAML Configuration**. 
   
    ![What is Azure AD Connect][13]

4. On the **SAML Configuration** page, perform the following steps: 

    ![What is Azure AD Connect][14]

     a. As **Unique Identifier**, select **NameID**.

     b. As **Unique Identifier Maps To**, select **Username**.
  
     c. To upload your **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)**, click **Browse** to select the file, and then **Upload File**.
 
     d. To test the configuration, click **Run Test**. 
    
	>[!NOTE]
    >You need to wait for the message "*The SAML test is complete. Please close this window*". Then, close the opened browser window. The **Enable SAML** checkbox is only enabled if the test has been completed. 
     
	 e. Select **Enable SAML**.
    
	 f. Click **Save Changes**. 





## Quick Reference

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**



## Additional Resources

* [How to integrate Halogen-Software with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-halogen-software-tutorial)

<!--Image references-->

[12]: ./media/tutorial_halogen_12.png

[13]: ./media/tutorial_halogen_13.png

[14]: ./media/tutorial_halogen_14.png