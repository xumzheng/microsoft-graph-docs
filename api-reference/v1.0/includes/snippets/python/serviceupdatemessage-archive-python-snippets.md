---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ArchivePostRequestBody();
requestBody.setMessageIds(['MC172851', 'MC167983', ]);



result = await client.admin().serviceAnnouncement().messages().archive().post(requestBody);


```