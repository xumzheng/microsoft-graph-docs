---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration(
query_params = MessagesRequestBuilderGetQueryParameters()
query_params.orderby = ["from/emailAddress/name desc","subject"]

)


result = await client.me.mailFolders_by_id('mailFolder-id').messages.get(request_config)


```