---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OutlookCategory();
requestBody.setColor(CategoryColor('preset15'));



requestResult = graphServiceClient.me().outlook().masterCategoriesById('outlookCategory-id').patch(requestBody);


```