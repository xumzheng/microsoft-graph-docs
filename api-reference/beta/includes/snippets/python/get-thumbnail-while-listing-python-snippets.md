---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ChildrenRequestBuilder.ChildrenRequestBuilderGetQueryParameters(
		expand = ["thumbnails"],
)

request_configuration = ChildrenRequestBuilder.ChildrenRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').children.get(request_configuration = request_configuration)


```