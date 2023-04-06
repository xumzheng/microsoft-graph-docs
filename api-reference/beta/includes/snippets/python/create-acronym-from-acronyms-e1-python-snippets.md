---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Acronym()
request_body.setDisplayName('DNN')

request_body.setStandsFor('Deep Neural Network')

request_body.setDescription('A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.')

request_body.setWebUrl('http://microsoft.com/deep-neural-network')

request_body.setState(AnswerState('draft'))



result = await client.search.acronyms.post(request_body, headers=)


```