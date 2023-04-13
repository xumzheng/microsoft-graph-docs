---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateSessionPostRequestBody()
request_body.persist_changes = True



request_configuration = CreateSessionRequestBuilder.CreateSessionRequestBuilderPostRequestConfiguration(
headers = {
		'Prefer' : "respond-async",
}

)


result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.createSession.post(request_body = request_body, request_configuration = request_configuration)


```