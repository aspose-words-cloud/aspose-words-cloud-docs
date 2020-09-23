---
title: "Aspose.Words for Cloud 17.7 Release Notes"
type: docs
url: /release-notes/2017/17-7/
aliases: [/aspose-words-for-cloud-17-7-release-notes/]
weight: 60
---

The page contains release notes for Aspose.Words for Cloud update 17.7. – [API Version 1.1](http://api.aspose.cloud/swagger/ui/index)

## Full List of Issues Covering all Changes in this Release

|Key|Summary|Category|
| :- | :- | :- |
|**WORDSCLOUD-204**|Mail Merge not generating output from templates|Bug|
|**WORDSCLOUD-209**|destFileName Description for mail merge is wrong|Bug|
|**WORDSCLOUD-191**|Formfields methods cleanup|Enhancement|
|**WORDSCLOUD-202**|Add pdf save option "DisplayDocTitle"|Enhancement|
|**WORDSCLOUD-201**|Add new save format "PCL"|Feature|
|**WORDSCLOUD-206**|Add support for PDF->Word conversion in API|Feature|

## Important Changes and New Features

#### Working with PDF documents

This release introduces support for reading PDF documents for the purpose of converting them to Word formats such as DOCX, DOC and working with them the same way as you would work with Word documents. User experience is consistent with other Aspose.Words API, now you can just specify PDF document name as input to Aspose.Words APIs.
Further information and limitations for PDF to Word conversion are available in [Working with PDF Documents](https://docs.aspose.com/display/wordscloud/Working+with+PDF+Documents).

#### New saving options

New saving format PCL and PDF saving option DisplayDocTitle are available through Aspose.Words for Cloud APIs.

#### Formfields API update

New API for getting all form fields in Word document is available:

GET /v{version}/words/{name}/{paragraphPath}/formfields

Other form field API descriptions were updated to match common Aspose.Words notation.

#### Swagger documentation improvements

Publically available Swagger description and UI has received updates and fixes that make trying out and integrating APIs easier than ever.

#### Deprecated parameters

*replaceResourcesHostTo* parameter is now deprecated and will be removed in future versions of the API. Please contact Support if you are using it.

