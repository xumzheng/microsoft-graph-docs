---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = OutlookCategory();
request_body.setColor(CategoryColor('preset15'));



result = await client.me().outlook().masterCategoriesById('outlookCategory-id').patch(request_body);


```