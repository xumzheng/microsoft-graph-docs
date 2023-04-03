---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OutlookTaskFolder();
requestBody.setName('Charity work');



result = awaitclient.me().outlook().taskFoldersById('outlookTaskFolder-id').patch(requestBody);


```