---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ContactFolder();
request_body.setParentFolderId('parentFolderId-value');

request_body.setDisplayName('displayName-value');



result = await client.me.contactFoldersById('contactFolder-id').patch(request_body);


```