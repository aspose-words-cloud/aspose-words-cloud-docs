---
title: "Using Cloud AutoMerge for Dynamics CRM"
type: docs
url: /using-cloud-automerge-for-dynamics-crm/
aliases: [/using-cloud-automerge-for-dynamics-crm/]
weight: 10
---

#### Create Template and Upload
Below are the steps to create and upload Template in CRM

- Open word and create a template.
- Insert MailMerge fields for data comming from CRM. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_1)

- Make sure that the Field name matches exactly with the CRM field. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_2)

- Templates are specific to use with individual entity. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_3)

- Once the Template is created, Open Document Template entity in CRM and Create a New record.
- Give the name of the template and attach the created document in the attachment. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_4)
#### How to Configure Workflow
This section shows how Aspose .NET AutoMerge can be used with a workflow.

- Open Settings -> Processes within CRM and hit New.
- Enter Name and Entity and select category as Workflow. (Make sure your template is designed for the same entity you have selected.)
- Use the window to create your own workflow.
- If you want to use “Aspose AutoMerge” functionality Go to Add Step – > Aspose AutoMerge

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_5)

- Here you will see all available options to use with Aspose AutoMerge:
#### Create Document
Select this option to create a new document based on the template.

- Give a meaningful name to the step.
- Hit Set Properties to define the settings. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_6)

- **Enable Logging**: It will log all the steps performed by the plugin. (we leave this functionality to be fulfilled by the user themselves in the source code, If you would like to use our Log functionality un-comment the code in Log function)
- **Product URI**: This contains the cloud product URI through which all the requests are processed.
- **App SID**: It is the application AppSID From the Cloud storage of Aspose.
- **App Key**: It is the App password Key from the cloud storage of Aspose.
- **Document Template**: Use this lookup field to select Template. This template would be the base of your generated document.
- **Delete Template From Cloud Storage**: If you already own Aspose License for Aspose.Words use this attribute to use the license to generate full version of the document.
- **Delete Generated Document From Cloud Storage**: If you already own Aspose License for Aspose.Words use this attribute to use the license to generate full version of the document.
  Please Note that the document is generated at this stage and attached to the Primary record of the workflow. (In this case, created document is attached to the Contact)
#### Attach to Email
Select this option to attach the created document to an email. This step is used with combination of "Send Email" described below. Please notice that you can select an existing email as well as you can create an email within your workflow.

- First Create an email message within workflow.
- Set some properties for the email.
- Add Step to Attach to Email and Give a meaningful name.
- Hit Set Properties to define the settings. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_7)

- **Enable Logging**: It will log all the steps performed by the plugin. (we leave this functionality to be fulfilled by the user themselves in the source code, If you would like to use our Log functionality un-comment the code in Log function)
- **Email**: Use this lookup to select an already created email. (The email can be from existing emails or created email under the same workflow)
- **Attachment**: Select the created Output Attachment file to attach to the email.
#### Attach To Letter
Select this option to attach the created document to a letter. Please notice that you can select an existing letter as well as you can create a letter within your workflow.

- First Create a letter within workflow.
- Set some properties for the letter.
- Add Step to Attach to letter and Give a meaningful name.
- Hit Set Properties to define the settings. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_8)

- **Enable Logging**: It will log all the steps performed by the plugin. (we leave this functionality to be fulfilled by the user themselves in the source code, If you would like to use our Log functionality un-comment the code in Log function)
- **Letter**: Use this lookup to select an already created letter. (The letter can be from existing letters or created letter under the same workflow)
- **Attachment**: Select the created Output Attachment file to attach to the letter.
#### Attach To Entity
Select this step if you want to attach the document to any record. Attach to any record works same like Attach to Email/Letter.

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_9)

- **Enable Logging:** It will log all the steps performed by the plugin.
- **Attachment:** Select the created Output Attachment file to attach to the Entity.
- **Entity Logical Name:** Provide the logical name of the Entity here. (Like: account, contact, lead etc)
- **Record Id:** Provide the Record Primary GUID here to which the document is attached. Please note that it will not create a copy of document but attach the provided document directly.
#### Send Email
Use this step to send the email, this is used with the Attach to Email step where the document is attached with the email and sent.

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_10)

- **Enable Logging:** It will log all the steps performed by the plugin.
- **Email:** select the email you want to send.
#### Generate Copy of Document
Use this step to generate a copy of Document. It is usually used when you want to keep the document with the primary record as well as attach it under any other record.

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_11)

- **Enable Logging:** It will log all the steps performed by the plugin.
- **Attachment:** Select the generated document.
#### Delete Temp Document
Select this step if you want to delete the generated document from the primary entity.

- Give name to the step.
- Hit set properties to define the settings. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_12)

- **Enable Logging**: It will log all the steps performed by the plugin. (we leave this functionality to be fulfilled by the user themselves in the source code, If you would like to use our Log functionality un-comment the code in Log function)
- **Attachment**: Select the created Output Attachment file.
#### Execute Workflow and Ouput
Execution of workflow is depends on what options you have selected while configuring the workflow.

- Open Contact record and click on Run Workflow. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_13)

- Select your workflow and click OK. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_14)

- Workflow is executed successfully.
- Under All Activities the email and letter records are found. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_15)

- Open Email and view the attachments. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_16)

- Download the attachment and open in Microsoft Word. You will see the document created from the template. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_17)

- Similarly, go back to All activities and you can see the same document attached under letter. 

![todo:image_alt_text](using-cloud-automerge-for-dynamics-crm_18)
