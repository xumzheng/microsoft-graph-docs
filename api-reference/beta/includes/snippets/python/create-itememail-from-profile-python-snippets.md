---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ItemEmail();
requestBody.setAddress('Innocenty.Popov@adventureworks.com');



result = await client.me().profile().emails().post(requestBody);


```