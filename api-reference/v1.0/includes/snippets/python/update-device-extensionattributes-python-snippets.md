---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Device();
additionalData = [
'extensionAttributes' => requestBody = ExtensionAttributes();
		requestBody.setExtensionAttribute1('BYOD-Device');


requestBody.setExtensionAttributes($extensionAttributes);

];
requestBody.setAdditionalData(additionalData);




result = await client.devicesById('device-id').patch(requestBody);


```