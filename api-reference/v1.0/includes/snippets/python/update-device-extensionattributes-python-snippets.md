---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Device()
additionalData = [
'extensionAttributes' => request_body = ExtensionAttributes()
		request_body.extensionAttribute1 = 'BYOD-Device'


request_body.extension_attributes = extensionAttributes

];
request_body.additionaldata(additionalData)





result = await client.devices_by_id('device-id').patch(request_body = request_body)


```