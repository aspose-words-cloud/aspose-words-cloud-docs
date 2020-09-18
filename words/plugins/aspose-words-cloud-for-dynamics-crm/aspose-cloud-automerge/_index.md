---
title: "Aspose Cloud AutoMerge"
type: docs
url: /aspose-cloud-automerge/
aliases: [/aspose-cloud-automerge/]
weight: 10
---

The Aspose AutoMerge is an open source add-on to be used with Microsoft Dynamics CRM. This add-on is capable of generating document using template and attaching them to Any Entity, Letter, sending emails, Generating Copy of document and upload document on cloud storage. Easily configure a workflow and generate documents from templates. Aspose .Cloud AutoMerge can be used with all versions of **Microsoft Dynamics CRM 2013, 2015 and CRM Online**.

Major features of this Addon are:

- Create Templates in Microsoft Word and Upload them in CRM.
- Create a Document in CRM using the templates.
- Allow users to Add OptionSet fields in the templates.
- Allow users to Add Lookup fields in the templates.
- Provide functionality to attach the generated document with letter.
- Provide functionality to attach the generated document with email.
- Provide functionality to attach the generated document to any entity.
- Provide functionality to send the email.
- Provide functionality to create a copy of document.
- Upload the document on Cloud Storage.
- Delete document when not required (usually used after uploading to Cloud or sending via email).
## System Requirements and Supported Platforms
### System Requirements
In order to install and use Aspose Cloud AutoMerge for Microsoft Dynamics CRM you need to have one of the following CRM version installed

- Microsoft Dynamics CRM 2013.
- Microsoft Dynamics CRM 2015.
- Microsoft Dynamics CRM Online.

Please feel free to contact us if you find any issues in installing or using this Add-on.
### Supported Platforms
This addon will work with all version of Microsoft Dynamics CRM:

- Microsoft Dynamics CRM 2013.
- Microsoft Dynamics CRM 2015.
- Microsoft Dynamics CRM Online.
## Support,Extend and Contribute
### Support
We offer free support. Anyone who uses our product, whether they have bought them or are using an evaluation, deserves our full attention and respect.

You can log any issues or suggestions related to Aspose Cloud AutoMerge using any of the following platforms:

- [Codeplex](https://goo.gl/7Gv4MP)
- [Github](https://goo.gl/od35Lg)
- [Sourceforge](https://goo.gl/jTKXSa)
- [Bitbucket](https://goo.gl/Squzfh)
### Extend and Contribute
You can download the latest source code at:

- Download from [CodePlex](https://asposecloudcrm.codeplex.com/SourceControl/latest#Aspose Cloud AutoMerge/Source Code/).
- Download from [GitHub](https://github.com/asposemarketplace/asposecloudcrm/tree/master/Aspose%20Cloud%20AutoMerge/Source%20Code).
- Download from [BitBucket](https://bitbucket.org/asposemarketplace/aspose-cloud-for-dynamics-crm/src/31f6d33af4cf318c36955b9871961efe42869ce4/Aspose%20Cloud%20AutoMerge/Source%20Code/?at=master).
- Download from [SourceForge](https://sourceforge.net/p/asposecloudfordynamicscrm/code/ci/master/tree/Aspose%20Cloud%20AutoMerge/Source%20Code).

Execute MailMerge on Cloud file:

```java

        private string ExecuteMailMerge(CloudAppConfig Config, string Xml)

        {

            try

            {

                string URIRequest = Config.ProductUri + "/words/" + Config.FileName + "/executeMailMerge";

                string URISigned = Sign(URIRequest, Config.AppSID, Config.AppKey);

                string outputFileName = null;

                using (Stream responseStream = ProcessCommand(URISigned, "POST", Xml, "xml"))

                {

                    string strResponse = null;

                    using (StreamReader reader = new StreamReader(responseStream))

                    {

                        strResponse = reader.ReadToEnd();

                    }

                    using (MemoryStream ms = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(strResponse)))

                    {

                        XPathDocument xPathDoc = new XPathDocument(ms);

                        XPathNavigator navigator = xPathDoc.CreateNavigator();

                        //get File Name

                        XPathNodeIterator nodes = navigator.Select("/SaaSposeResponse/Document/FileName");

                        nodes.MoveNext();

                        outputFileName = nodes.Current.InnerXml;

                        return outputFileName;

                    }

                }

            }

            catch (Exception ex)

            {

                throw ex;

            }

        }

```
## Installation and Usage
### Downloading,Installing or Uninstalling
#### Downloading
You can download Aspose Cloud AutoMerge 2.0.0.2015 for CRM from one of the following locations:

- [Codeplex](http://goo.gl/9LLjhP)
- [Github](http://goo.gl/Az00wC)
- [Sourceforge](http://goo.gl/jWo7jY)
- [Bitbucket](http://goo.gl/mC5Psb)

You can download Aspose Cloud AutoMerge 2.0.0.2013 for CRM from one of the following locations:

- [Codeplex](http://goo.gl/7Uy3v6)
- [Github](http://goo.gl/Kg4G6E)
- [Sourceforge](http://goo.gl/jWo7jY)
- [Bitbucket](http://goo.gl/mC5Psb)

You can download Aspose Cloud AutoMerge 1.0.0 for CRM from one of the following locations:

- [Codeplex](http://goo.gl/VfcGTd)
- [Github](http://goo.gl/7QOJlI)
- [Sourceforge](http://goo.gl/2rEubq)
- [Bitbucket](http://goo.gl/blUMuZ)
- [Code.MSDN](http://goo.gl/p0QEnp)
#### Installing Aspose Cloud AutoMerge
It is simple to install Aspose Cloud AutoMerge. Please follow below Instructions:

- Download the Solution File.
- Open CRM and go to Import Solution.
- Click Browse and select the downloaded solution file and click next.
- Click Next and wait for the solution to import.
- Click close when the solution is imported successfully.
#### Applying License
- Create an account on <http://cloud.aspose.com/> and Save its AppSID and AppKey.
- It will be later used in workflow configuration.
#### Uninstalling Aspose Cloud AutoMerge
- Go to solution and select "Aspose Cloud AutoMerge".
- Press the Delete button.
### Using
﻿[Using Cloud AutoMerge for Dynamics CRM](/using-cloud-automerge-for-dynamics-crm/)
