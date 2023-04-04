---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Device();
additionalData = [
'extensionAttributes' => request_body = ExtensionAttributes();
		request_body.setExtensionAttribute1('BYOD-Device');


request_body.setExtensionAttributes($extensionAttributes);

];
request_body.setAdditionalData(additionalData);




result = await client.devicesById('device-id').patch(request_body);


```