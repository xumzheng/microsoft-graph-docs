---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ContactFolder();
requestBody.setParentFolderId('parentFolderId-value');

requestBody.setDisplayName('displayName-value');



result = awaitclient.me().contactFoldersById('contactFolder-id').patch(requestBody);


```