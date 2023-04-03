---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OutlookTaskFolder();
requestBody.setName('Cooking');



result = awaitclient.me().outlook().taskGroupsById('outlookTaskGroup-id').taskFolders().post(requestBody);


```