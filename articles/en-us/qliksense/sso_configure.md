## Prerequisites

To configure Azure AD integration with Qlik Sense Enterprise, you need the following items:

- An Azure AD subscription
- A Qlik Sense Enterprise single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Qlik Sense Enterprise for single sign-on

1. Navigate to the Qlik Sense Qlik Management Console (QMC) as a user who can create virtual proxy configurations.

2. In the QMC, click on the **Virtual Proxies** menu item.
   
    ![QlikSense][qs6] 

3. At the bottom of the screen, click the **Create new** button.
   
    ![QlikSense][qs7]

4. The Virtual proxy edit screen appears.  On the right side of the screen is a menu for making configuration options visible.
   
    ![QlikSense][qs9]

5. With the Identification menu option checked, enter the identifying information for the Azure virtual proxy configuration.
    
    ![QlikSense][qs8]  
    
    a. The **Description** field is a friendly name for the virtual proxy configuration.  Enter a value for a description.
    
    b. The **Prefix** field identifies the virtual proxy endpoint for connecting to Qlik Sense with Azure AD Single Sign-On.  Enter a unique prefix name for this virtual proxy.
    
    c. **Session inactivity timeout (minutes)** is the timeout for connections through this virtual proxy.
    
    d. The **Session cookie header name** is the cookie name storing the session identifier for the Qlik Sense session a user receives after successful authentication.  This name must be unique.

6. Click on the Authentication menu option to make it visible.  The Authentication screen appears.
    
    ![QlikSense][qs10]
    
    a. The **Anonymous access mode** drop down determines if anonymous users may access Qlik Sense through the virtual proxy.  The default option is No anonymous user.
    
    b. The **Authentication method** drop-down determines the authentication scheme the virtual proxy will use.  Select SAML from the drop-down list.  More options appear as a result.
    
    c. In the **SAML host URI field**, input the hostname users enter to access Qlik Sense through this SAML virtual proxy.  The hostname is the uri of the Qlik Sense server.
    
    d. In the **SAML entity ID**, enter the same value entered for the SAML host URI field.
    
    e. The **SAML IdP metadata** is the file edited earlier in the **Edit Federation Metadata from Azure AD Configuration** section.  **Before uploading the IdP metadata, the file needs to be edited** to remove information to ensure proper operation between Azure AD and Qlik Sense server.  **Please refer to the instructions above if the file has yet to be edited.**  If the file has been edited click on the Browse button and select the edited metadata file to upload it to the virtual proxy configuration.
    
    f. Enter the attribute name or schema reference for the SAML attribute representing the **UserID** Azure AD sends to the Qlik Sense server.  Schema reference information is available in the Azure app screens post configuration.  To use the name attribute, `enter http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name`.
    
    g. Enter the value for the **user directory** that will be attached to users when they authenticate to Qlik Sense server through Azure AD.  Hardcoded values must be surrounded by **square brackets []**.  To use an attribute sent in the Azure AD SAML assertion, enter the name of the attribute in this text box **without** square brackets.
    
    h. The **SAML signing algorithm** sets the service provider (in this case Qlik Sense server) certificate signing for the virtual proxy configuration.  If Qlik Sense server uses a trusted certificate generated using Microsoft Enhanced RSA and AES Cryptographic Provider, change the SAML signing algorithm to **SHA-256**.
    
    i. The SAML attribute mapping section allows for additional attributes like groups to be sent to Qlik Sense for use in security rules.

7. Click on the **LOAD BALANCING** menu option to make it visible.  The Load Balancing screen appears.
    
    ![QlikSense][qs11]

8. Click on the **Add new server node** button, select engine node or nodes Qlik Sense will send sessions to for load balancing purposes, and click the **Add** button.
    
    ![QlikSense][qs12]

9. Click on the Advanced menu option to make it visible. The Advanced screen appears.
    
    ![QlikSense][qs13]
    
    The Host white list identifies hostnames that are accepted when connecting to the Qlik Sense server.  **Enter the hostname users will specify when connecting to Qlik Sense server.** The hostname is the same value as the SAML host uri without the https://.

10. Click the **Apply** button.
    
    ![QlikSense][qs14]

11. Click OK to accept the warning message that states proxies linked to the virtual proxy will be restarted.
    
    ![QlikSense][qs15]

12. On the right side of the screen, the Associated items menu appears.  Click on the **Proxies** menu option.
    
    ![QlikSense][qs16]

13. The proxy screen appears.  Click the **Link** button at the bottom to link a proxy to the virtual proxy.
    
    ![QlikSense][qs17]

14. Select the proxy node that will support this virtual proxy connection and click the **Link** button.  After linking, the proxy will be listed under associated proxies.
    
    ![QlikSense][qs18]
  
    ![QlikSense][qs19]

15. After about five to ten seconds, the Refresh QMC message will appear.  Click the **Refresh QMC** button.
    
    ![QlikSense][qs20]

16. When the QMC refreshes, click on the **Virtual proxies** menu item. The new SAML virtual proxy entry is listed in the table on the screen.  Single click on the virtual proxy entry.

    ![QlikSense][qs51]

17. At the bottom of the screen, the Download SP metadata button will activate.  Click the **Download SP metadata** button to save the metadata to a file.
    
    ![QlikSense][qs52]

18. Open the sp metadata file.  Observe the **entityID** entry and the **AssertionConsumerService** entry.  These values are equivalent to the **Identifier** and the **Sign on URL** in the Azure AD application configuration. Paste these values in the **Qlik Sense Enterprise Domain and URLs** section in the Azure AD application configuration if they are not matching, then you should replace them in the Azure AD App configuration wizard.
    
    ![QlikSense][qs53]

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Qlik Sense Enterprise with Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-qliksense-enterprise-tutorial)

<!--Image references-->

[qs6]: ./media/tutorial_qliksenseenterprise_06.png
[qs7]: ./media/tutorial_qliksenseenterprise_07.png
[qs8]: ./media/tutorial_qliksenseenterprise_08.png
[qs9]: ./media/tutorial_qliksenseenterprise_09.png
[qs10]: ./media/tutorial_qliksenseenterprise_10.png
[qs11]: ./media/tutorial_qliksenseenterprise_11.png
[qs12]: ./media/tutorial_qliksenseenterprise_12.png
[qs13]: ./media/tutorial_qliksenseenterprise_13.png
[qs14]: ./media/tutorial_qliksenseenterprise_14.png
[qs15]: ./media/tutorial_qliksenseenterprise_15.png
[qs16]: ./media/tutorial_qliksenseenterprise_16.png
[qs17]: ./media/tutorial_qliksenseenterprise_17.png
[qs18]: ./media/tutorial_qliksenseenterprise_18.png
[qs19]: ./media/tutorial_qliksenseenterprise_19.png
[qs20]: ./media/tutorial_qliksenseenterprise_20.png
[qs51]: ./media/tutorial_qliksenseenterprise_51.png
[qs52]: ./media/tutorial_qliksenseenterprise_52.png
[qs53]: ./media/tutorial_qliksenseenterprise_53.png