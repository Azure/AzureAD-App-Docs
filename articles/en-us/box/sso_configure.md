##Configuring Box for single sign-on

The objective of this section is to outline how to enable users to authenticate to Box with their account in Azure AD using federation based on the SAML protocol. <br>
As part of this procedure, you are required to upload metadata to Box.com.

###To configure single sign-on, perform the following steps:

1.  First, ensure that the **Sign-on URL** is set appropriately for Box in the Azure management portal. This is the URL of your Box.com tenant and should follow the format: https://<mydomainname>.box.com. 

2.  Second, ensure a valid **SAML signing certificate** has been created for Box in the Azure management portal.

3.  To begin configuring your Box.com tenant to use Azure Active Directory as an identity provider, start by downloading the following metadata file, and saving it locally on your computer: [Download metadata file](%metadata:MetadataDownloadUrl%)

4.  Forward that metadata file to Box support team. The support team configures single sign-on for you.
