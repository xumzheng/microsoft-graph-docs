---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Acronym()
request_body.setDescription('A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.')



result = await client.search.acronyms_by_id('acronym-id').patch(request_body)


```