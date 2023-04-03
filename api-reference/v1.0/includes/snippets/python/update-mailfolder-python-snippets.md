---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MailFolder();
requestBody.setDisplayName('displayName-value');



result = awaitclient.me().mailFoldersById('mailFolder-id').patch(requestBody);


```