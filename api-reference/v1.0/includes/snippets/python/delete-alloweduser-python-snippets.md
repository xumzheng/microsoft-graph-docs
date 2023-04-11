---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RefRequestBuilderDeleteRequestConfiguration(
)


await client.print.shares_by_id('printerShare-id').allowedUsers_by_id('user-id').ref.delete()


```