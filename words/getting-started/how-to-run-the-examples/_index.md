---
title: "How to Run the Examples"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/how-to-run-the-examples/
aliases: [/how-to-run-the-examples/]
description: "Code examples for Aspose.Words Cloud — convert documents, process text, and more with Python and cURL."
weight: 130
---

All examples are hosted on [GitHub](https://github.com/aspose-words-cloud). Each SDK repository includes working code samples.

## Quick Example — Convert DOCX to PDF

```bash
# Get access token
TOKEN=$(curl -s -X POST "https://api.aspose.cloud/connect/token" \
  -d "grant_type=client_credentials&client_id=$CLIENT_ID&client_secret=$CLIENT_SECRET" \
  -H "Content-Type: application/x-www-form-urlencoded" \
  | grep -o '"access_token":"[^"]*"' | cut -d'"' -f4)

# Convert document
curl -X PUT "https://api.aspose.cloud/v4.0/words/test.docx/saveAs" \
  -H "Authorization: Bearer $TOKEN" \
  -H "Content-Type: application/json" \
  -d '{"SaveFormat":"pdf", "FileName":"test.pdf"}'
```

```python
import asposewordscloud

api = asposewordscloud.WordsApi("CLIENT_ID", "CLIENT_SECRET")

# Upload a document
with open("test.docx", "rb") as f:
    api.upload_file(asposewordscloud.models.requests.UploadFileRequest(
        f, "test.docx"))

# Convert to PDF
request = asposewordscloud.models.requests.SaveAsRequest(
    "test.docx",
    asposewordscloud.models.SaveOptionsData(
        save_format="pdf", file_name="test.pdf"
    )
)
result = api.save_as(request)
print(f"Converted: {result.save_result.dest_document.href}")
```

→ [All SDK Repositories on GitHub](https://github.com/aspose-words-cloud)  |  → [Quickstart](/words/getting-started/quickstart/)
