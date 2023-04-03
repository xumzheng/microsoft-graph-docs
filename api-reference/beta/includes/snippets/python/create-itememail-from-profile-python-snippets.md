---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ItemEmail();
requestBody.setAddress('Innocenty.Popov@adventureworks.com');



result = awaitclient.me().profile().emails().post(requestBody);


```