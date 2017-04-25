
## Prerequisites

To configure Azure AD integration with Zscaler ZSCloud, you need the following items:

- An Azure AD subscription
- A Zscaler ZSCloud single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Zscaler ZSCloud for single sign-on

1. In a different web browser window, log in to your ZScaler ZSCloud company site as an administrator.

2. In the menu on the top, click **Administration**.
   
   ![Administration](./media/IC800206.png "Administration")

3. Under **Manage Administrators & Roles**, click **Manage Users & Authentication**.   
   			
	![Manage Users & Authentication](./media/IC800207.png "Manage Users & Authentication")

4. In the **Choose Authentication Options for your Organization** section, perform the following steps:   
   				
	![Authentication](./media/IC800208.png "Authentication")
   
    a. Select **Authenticate using SAML Single Sign-On**.

    b. Click **Configure SAML Single Sign-On Parameters**.
  
5.  On the **Configure SAML Single Sign-On Parameters** dialog page, perform the following steps, and then click **Done**:   
   
	![Single Sign-On](./media/IC800209.png "Single Sign-On")
   
6. Paste the **SAML Single Sign-On Service URL** value into the **URL of the SAML Portal to which users are sent for authentication** textbox.

7. In the **Attribute containing Login Name** textbox, type **NameID**.

8. To upload your downloaded certificate, click **Zscaler pem**.

9. Select **Enable SAML Auto-Provisioning**.

10. On the **Configure User Authentication** dialog page, perform the following steps:

    ![Administration](./media/IC800210.png "Administration")
    
    a. Click **Save**.

    b. Click **Activate Now**.

## Configuring proxy settings
### To configure the proxy settings in Internet Explorer
1. Start **Internet Explorer**.
2. To open the **Internet Options** dialog, Select **Internet options** from the **Tools** menu.   
  	
	 ![Internet Options](./media/IC769492.png "Internet Options")

3. Click the **Connections** tab.   
  
	 ![Connections](./media/IC769493.png "Connections")

4. Click **LAN settings** to open the **LAN Settings** dialog.

5. In the Proxy server section, perform the following steps:   
   
	![Proxy server](./media/IC769494.png "Proxy server")

    a. Select Use a proxy server for your LAN.

    b. In the Address textbox, type **gateway.zscalerone.net**.

    c. In the Port textbox, type **80**.

    d. Select **Bypass proxy server for local addresses**.

    e. Click **OK** to close the **Local Area Network (LAN) Settings** dialog.

6. Click **OK** to close the **Internet Options** dialog.


## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certificate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**


