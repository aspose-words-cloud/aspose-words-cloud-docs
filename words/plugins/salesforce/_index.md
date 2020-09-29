---
title: "Aspose.Words Cloud for SalesForce"
type: docs
url: /plugins/salesforce/
aliases: [/aspose-words-cloud-for-salesforce/]
description: "Aspose.Words Cloud for Salesforce"
weight: 20
---

Apex is a strongly typed, object-oriented programming language that allows developers to execute flow and transaction control statements on the Force.com platform server in conjunction with calls to the Force.com​ API.

## Aspose.Words Cloud for Salesforce

Aspose.Words for Salesforce allows APEX and Force.com developers to work with Aspose’s REST API. Integrating Aspose.Words Cloud for Salesforce into your Salesforce app is simple and effective. It’s a cloud solution, so you don’t have to install anything, and it integrates with other cloud services too. Aspose.Words Cloud for Salesforce provides you the ability to use all the document processing features right inside the Salesforce platform painlessly.

Aspose.Words Cloud for Salesforce is a series of examples we provide to our users to easily manipulate documents on Salesforce platform using Aspose Cloud APIs.

Along with this project we’ve also set up salesforce package which you can install on your Salesforce platform.

- [Aspose.Words sample](https://ap1.salesforce.com/packaging/installPackage.apexp?p0=04t900000002D7B).

## System Requirements

In order to use "Aspose.Words Cloud for Salesforce" you need have below listed items.

- Force.com IDE

[Click Here](http://wiki.developerforce.com/page/Force.com_IDE_Installation) for the installation guide of Force.com IDE.
Please feel free to contact us if you find any issues in installing or using this plugin.

## Supported Platforms

It supports salesforce's "Force.com" platform.

\- Force.com is a platform as a service (PaaS) that allows developers to create multitenant add-on applications that integrate into the main Salesforce.com application. Force.com applications are hosted on Salesforce.com's infrastructure.

## Support, Extend and Contribute

We believe the key to success lies in our ability to support and establish mutually beneficial long-term relationships with our customers. Our experts are here to answer your questions, help you troubleshoot issues, improve your experience and increase satisfaction with our products. If you have any questions and need support on Aspose Cloud for Salesforce you can log them using any of the following platforms.

- [Github](https://github.com/asposemarketplace/Aspose_for_Salesforce/issues).

## Installation

### Downloading

You can download the Aspose.Words Cloud for Salesforce from one of the following locations:

- Download from [Github](https://github.com/asposemarketplace/Aspose_for_SalesForce/archive/master.zip).

### Installing

Once downloaded, please follow these steps to deploy Aspose.Words Cloud on Salesforce:

### Import Aspose.Words Cloud for Salesforce as project in Eclipse as Force.com project

- File > Import General > Existing Projects into Workspace
- Select the Aspose_for_SalesForce/Aspose.Words Sample unziped folder as root directory.

### Deploy on Salesforce

- Right Click on Project > Force.com > Deploy to Server.

### Using

After you have installed the Aspose.Words Cloud for Salesforce it is really simple to start using it.
Please follow these steps to get started:

- Login to your Salesforce Account on www.salesforce.com.
- Open Build > Develop > Pages.
- Click on Preview AsposeCloudHome in New Window.
- Register / Login Aspose Account.
- Upload following files to your aspose account [TestMailMerge.doc](https://dl.dropbox.com/u/5464471/TestMailMerge.doc) and [mail_merge_data.xml](https://dl.dropbox.com/u/5464471/mail_merge_data.xml).
- Fill the form on AsposeCloudHome page.
- Make sure you have api.aspose.com/v1.1 enabled under your Remote Site Settings.

## Code Sample

### Visualforce Page

**MailMerge.page**

```HTML
<apex:page controller="MailMergeController">
<apex:form id="theForm">
    <apex:pageBlock title="Requirements" rendered="true">
        <ol>
            <li>Register aspose account.</li>
            <li>Fill in the form below and click Run Sample (all fields are required).</li>
        </ol>
    </apex:pageBlock>
    <apex:pageBlock title="Execute Mail Merge Template in Salesforce" rendered="true">
        <table>
            <tr>
                <td><b>App SID:</b></td>
                <td><apex:inputText value="{!appSID}" size="100"/></td>
            </tr>
            <tr>
                <td><b>App Key:</b></td>
                <td><apex:inputText value="{!appKey}" size="100"/></td>
            </tr>
            <tr>
                <td><b>File Name:</b></td>
                <td><apex:inputText value="{!fileName}" size="100"/></td>
            </tr>
            <tr>
                <td><b>Data File Name:</b></td>
                <td><apex:inputText value="{!dataFileName}" size="100"/></td>
            </tr>
            <tr>
                <td><b>Save Format:</b> (pdf,tiff,html)</td>
                <td><apex:inputText value="{!saveFormat}" size="100"/></td>
            </tr>
        </table>
        <div class="container">
            <apex:commandButton action="{!runSample}" value="Run Sample" /><br/>
            <p>
                <span>Output: </span>
                <apex:outputLabel >{!output}</apex:outputLabel>
            </p>
        </div>
    </apex:pageBlock>
</apex:form>
</apex:page>
```

### Controller Class

**MailMergeController.cls**

```JAVA
public with sharing class MailMergeController {
    public string appSID {get; set;}
    public string appKey {get; set;}
    public string fileName {get; set;}
    public string dataFileName {get; set;}
    public string saveFormat {get; set;}
    public string output {get; set;}

    public PageReference runSample() {
        Product.BaseProductUri = 'http://api.aspose.com/v1.1';
        AsposeCloudApp.setAppInfo(appKey, appSID);
        MailMerge api = new MailMerge();
        String downloadURL = api.ExecuteMailMerege(fileName,dataFileName,saveFormat);
        this.output = downloadURL;
        return null;
    }
}
```

### MailMerge Class

**MailMerge.cls**

```JAVA
public with sharing class MailMerge {
    public string apiResponse {get; set;}
    public String ExecuteMailMerege(String FileName, String dataFile, SaveFormat outFormat) {
        return ExecuteMailMerege(FileName, dataFile, String.valueOf(outFormat));
    }
    public String ExecuteMailMerege(String FileName, String dataFile, String outFormat) {
        try {
            //build URI to get Image
            String strURI = Product.BaseProductUri + '/words/' + FileName + '/executeMailMerge?mailMergeDataFile=' + dataFile;
            String signedURI = Utils.Sign(strURI);
            system.debug('Signed URI = ' + signedURI);
            String strJSON = Utils.ProcessCommand(signedURI, 'POST', null, 'json');
            this.apiResponse = strJSON;
            system.debug(strJSON);

            //prepare signed download link
            String downloadURL = null;
            Map<String, Object> params = (Map<String, Object>) JSON.deserializeUntyped(strJSON);
            if(params.containsKey('Document')){
                Map<String, Object> doc = (Map<String, Object>) params.get('Document');
                String DocName = (String) doc.get('FileName');
                strURI = Product.BaseProductUri + '/words/' + DocName + '?format=' + outFormat;
                downloadURL = Utils.Sign(strURI);
            }
            return downloadURL;
        }
        catch (Exception ex) {
            system.debug(ex);
            return null;
        }
    }
}
```

### Utility Classes

**Product.cls**

```JAVA
public with sharing class Product {
    public static String BaseProductUri { get; set; }
}
```

**AsposeCloudApp.cls**

```JAVA
public with sharing class AsposeCloudApp {
    public static String AppSID { get; set; }
    public static String AppKey { get; set; }
    public static void setAppInfo(String key, String sid) {
        AppSID=sid;
        AppKey=key;
    }
}
```

**Utils.cls**

```JAVA
public with sharing class Utils {
    public static String Sign(String data) {
        String HMAC_SHA1 = 'HmacSHA1';

        try {
            data = data.replace(' ', '%20');
            URL url = new URL(data);
            String path = url.getPath();
            path = path.replace(' ', '%20');

            // Remove final slash here as it can be added automatically.
            path = path.removeEnd('/');
            String filePart = url.getPath() + (url.getQuery() == null ? '?' : '?' + url.getQuery()) + '&appSID=' + AsposeCloudApp.AppSID;
            url = new URL(url.getProtocol(), url.getHost(), url.getPort(), filePart);

            // compute the hmac on input data bytes
            Blob mac = Crypto.generateMac(HMAC_SHA1, Blob.valueOf(url.toExternalForm()), Blob.valueOf(AsposeCloudApp.AppKey));
            String base64 = EncodingUtil.base64Encode(mac);
            system.debug('base64: ' + base64);

            // Remove invalid symbols.
            String result = base64.substring(0, base64.length() - 1);
            result = EncodingUtil.urlEncode(result, 'UTF-8');
            system.debug('signature: ' + result);
            String encodedUrl = url.toExternalForm() + '&signature=' + result;
            system.debug('full URL: ' + encodedUrl);
            return encodedUrl;
        } catch (Exception ex) {
            system.debug(ex.getStackTraceString());
            return null;
        }
    }
    public static String ProcessCommand(String strURI, String strHttpCommand, Blob content, String ContentType) {
        try {
            HttpRequest request = new HttpRequest();
            Integer len = 0;
            if (strContent != null) {
                request.setBodyAsBlob(content);
            }
            request.setEndpoint(strURI);
            request.setMethod(strHttpCommand);
            if (ContentType.toLowerCase() == 'xml').
                request.setHeader('Content-Type', 'application/xml');
            else
                request.setHeader('Content-Type', 'application/json');
            request.setHeader('Accept', 'application/json');
            //request.setTimeout(Timeout);
            Http http = new Http();
            HttpResponse res = http.send(request);
            return res.getBody();
        } catch (Exception ex) {
            system.debug('HTTP ERROR' + ex.getMessage());
            system.debug(ex.getStackTraceString());
            return null;
        }
    }
}
```
