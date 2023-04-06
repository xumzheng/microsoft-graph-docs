---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookCategory()
request_body.setColor(CategoryColor('preset15'))


request_config = OutlookCategoryRequestBuilderPatchRequestConfiguration(
request_config = OutlookCategoryRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.outlook.masterCategories_by_id('outlookCategory-id').patch(request_body, headers=)


```