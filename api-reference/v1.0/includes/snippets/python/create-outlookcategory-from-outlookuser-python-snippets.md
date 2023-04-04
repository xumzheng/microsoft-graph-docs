---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = OutlookCategory();
request_body.setDisplayName('Project expenses');

request_body.setColor(CategoryColor('preset9'));



result = await client.me.outlook.masterCategories.post(request_body);


```