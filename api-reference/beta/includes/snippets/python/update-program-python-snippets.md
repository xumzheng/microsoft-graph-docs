---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Program();
requestBody.setDisplayName('testprogram3 new name');



result = awaitclient.programsById('program-id').patch(requestBody);


```