---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Program()
request_body.displayName = 'testprogram3 new name'



request_configuration = ProgramRequestBuilderPatchRequestConfiguration(
)


result = await client.programs_by_id('program-id').patch(request_body = request_body)


```