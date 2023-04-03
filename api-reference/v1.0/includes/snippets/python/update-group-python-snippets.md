---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Group();
requestBody.setDescription('Library Assist');

requestBody.setDisplayName('Library Assist');

requestBody.setGroupTypes(['Unified', ]);

requestBody.setMailEnabled(true);

requestBody.setMailNickname('library-help');



requestResult = graphServiceClient.groupsById('group-id').patch(requestBody);


```