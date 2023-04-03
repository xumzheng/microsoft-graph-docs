---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityUserFlowAttribute();
requestBody.setDisplayName('Hobby');

requestBody.setDescription('Your hobby');

requestBody.setDataType(IdentityUserFlowAttributeDataType('string'));



requestResult = graphServiceClient.identity().userFlowAttributes().post(requestBody);


```