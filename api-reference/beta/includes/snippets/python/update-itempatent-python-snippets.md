---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ItemPatent();
requestBody.setNumber('USPTO-3954432633');

requestBody.setWebUrl('https://patents.gov/3954432633');



requestResult = graphServiceClient.usersById('user-id').profile().patentsById('itemPatent-id').patch(requestBody);


```