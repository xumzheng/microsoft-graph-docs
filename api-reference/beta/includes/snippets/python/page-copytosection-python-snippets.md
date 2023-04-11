---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyToSectionPostRequestBody()
request_body.id = 'id-value'

request_body.groupId = 'groupId-value'



request_configuration = CopyToSectionRequestBuilderPostRequestConfiguration(
)


result = await client.me.onenote.pages_by_id('onenotePage-id').copyToSection.post(request_body = request_body)


```