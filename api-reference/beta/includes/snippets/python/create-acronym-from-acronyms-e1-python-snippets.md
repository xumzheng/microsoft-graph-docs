---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Acronym()
request_body.displayName = 'DNN'

request_body.standsFor = 'Deep Neural Network'

request_body.description = 'A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.'

request_body.webUrl = 'http://microsoft.com/deep-neural-network'

request_body.State(AnswerState('draft'))



request_configuration = AcronymsRequestBuilderPostRequestConfiguration(
)


result = await client.search.acronyms.post(request_body = request_body)


```