---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OutlookTaskFolder();
requestBody.setName('Volunteer');



requestResult = graphServiceClient.me().outlook().taskFolders().post(requestBody);


```