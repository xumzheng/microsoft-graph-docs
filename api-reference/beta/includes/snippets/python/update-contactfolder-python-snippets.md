---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ContactFolder();
requestBody.setParentFolderId('parentFolderId-value');

requestBody.setDisplayName('displayName-value');



result = await client.me().contactFoldersById('contactFolder-id').patch(requestBody);


```