## Prerequisites

To configure Azure AD integration with PerformanceCentre, you need the following items:

- An Azure AD subscription
- A PerformanceCentre single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring PerformanceCentre for single sign-on

1. Sign-on to your **PerformanceCentre** company site as administrator.

2. In the tab on the left side, click **Configure**.
   
    ![Azure AD Single Sign-On][10]

3. In the tab on the left side, click **Miscellaneous**, and then click **Single Sign On**.
   
    ![Azure AD Single Sign-On][11]

4. As **Protocol**, select **SAML**.
   
    ![Azure AD Single Sign-On][12]

5. Open your **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)** in notepad, copy the content, paste it into the **Identity Provider Metadata** textbox, and then click **Save**.
   
    ![Azure AD Single Sign-On][13]

6. Verify that the values for the **Entity Base URL** and **Entity ID URL** are correct.
    
     ![Azure AD Single Sign-On][14]

## Quick Reference

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate PerformanceCentre with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-performancecentre-tutorial)

<!--Image references-->

[10]: ./media/tutorial_performancecentre_06.png
[11]: ./media/tutorial_performancecentre_07.png
[12]: ./media/tutorial_performancecentre_08.png
[13]: ./media/tutorial_performancecentre_09.png
[14]: ./media/tutorial_performancecentre_10.png