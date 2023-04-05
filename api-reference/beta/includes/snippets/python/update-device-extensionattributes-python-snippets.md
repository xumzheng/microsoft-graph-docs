---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Device()
extensionAttributes = OnPremisesExtensionAttributes()
extensionAttributes.setExtensionAttribute1('BYOD-Device')


request_body.setExtensionAttributes($extensionAttributes)


result = await client.devicesby_id('device-id').patch(request_body)


```