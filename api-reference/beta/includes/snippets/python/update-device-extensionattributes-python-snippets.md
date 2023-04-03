---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Device();
extensionAttributes = OnPremisesExtensionAttributes();
extensionAttributes.setExtensionAttribute1('BYOD-Device');


requestBody.setExtensionAttributes($extensionAttributes);


requestResult = graphServiceClient.devicesById('device-id').patch(requestBody);


```