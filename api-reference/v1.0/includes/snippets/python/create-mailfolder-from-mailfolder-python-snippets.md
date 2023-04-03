---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = MailFolder();
requestBody.setDisplayName('displayName-value');

requestBody.setIsHidden(true);



requestResult = graphServiceClient.me().mailFoldersById('mailFolder-id').childFolders().post(requestBody);


```