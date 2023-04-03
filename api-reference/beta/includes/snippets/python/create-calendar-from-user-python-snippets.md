---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Calendar();
requestBody.setName('Volunteer');



requestResult = graphServiceClient.me().calendars().post(requestBody);


```