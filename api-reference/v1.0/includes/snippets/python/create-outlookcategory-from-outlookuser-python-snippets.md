---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OutlookCategory();
requestBody.setDisplayName('Project expenses');

requestBody.setColor(CategoryColor('preset9'));



result = await client.me().outlook().masterCategories().post(requestBody);


```