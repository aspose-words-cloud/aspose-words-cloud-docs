---
title: "Aspose.Words Cloud 19.12 Release Notes"
type: docs
url: /aspose-words-cloud-19-12-release-notes/
weight: 10
---

## **Important Changes and New Features**
### **API Changes**
1. Fixed issue with "borderType" parameter in "border" endpoints in swagger and SDKs
1. Increased max size of uploaded files (now it is 100mb).
### **PDF to Word conversion improvements**
- improved default font replacement logic;
- an OutOfMemory error doesn't occur on large documents anymore;
- added support for more color spaces (CalGrey, CalRGB, Lab).
### **Bug Fixes**

|WORDSCLOUD-960|Incorrect "borderType" parameter name in swagger|Bug|
| :- | :- | :- |
|WORDSCLOUD-992|Uploading a large file throws request body too large exception|Bug|
### **Aspose.Words Cloud Android SDK**
- ColorMode property has been moved from SaveOptionsData to FixedPageSaveOptionsData
