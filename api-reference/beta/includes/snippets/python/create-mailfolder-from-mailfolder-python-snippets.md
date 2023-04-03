---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = MailFolder();
requestBody.setDisplayName('displayName-value');

requestBody.setIsHidden(true);



result = await client.me().mailFoldersById('mailFolder-id').childFolders().post(requestBody);


```