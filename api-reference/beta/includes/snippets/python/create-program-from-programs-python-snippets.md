---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Program()
request_body.displayName = 'testprogram3'

request_body.description = 'test description'



request_configuration = ProgramsRequestBuilderPostRequestConfiguration(
)


result = await client.programs.post(request_body = request_body)


```