---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AudioRoutingGroup()
request_body.setId('oneToOne')

request_body.setRoutingMode(RoutingMode('onetoone'))

request_body.setSources(['632899f8-2ea1-4604-8413-27bd2892079f', ])

request_body.setReceivers(['550fae72-d251-43ec-868c-373732c2704f', '72f988bf-86f1-41af-91ab-2d7cd011db47', ])



result = await client.communications.calls._by_id('call-id').audioRoutingGroups._by_id('audioRoutingGroup-id').patch(request_body)


```