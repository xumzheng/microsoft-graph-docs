---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Tag();
requestBody.setDescription('This is an updated description.');



result = awaitclient.compliance().ediscovery().casesById('case-id').tagsById('tag-id').patch(requestBody);


```