---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Device()
extensionAttributes = OnPremisesExtensionAttributes()
extensionAttributes.extensionAttribute1 = 'BYOD-Device'


request_body.extensionAttributes = extensionAttributes



result = await client.devices_by_id('device-id').patch(request_body = request_body)


```