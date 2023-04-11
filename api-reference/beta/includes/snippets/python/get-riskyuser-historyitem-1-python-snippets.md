---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RiskyUserHistoryItemRequestBuilderGetRequestConfiguration(
)


result = await client.riskyUsers_by_id('riskyUser-id').history_by_id('riskyUserHistoryItem-id').get()


```