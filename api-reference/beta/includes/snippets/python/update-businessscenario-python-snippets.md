---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BusinessScenario();
requestBody.setOwnerAppIds(['44109254-4b2b-7a33-76ee-c890a167b295', '13eb9d8b-1d63-4153-9417-3a69ab200a78', ]);



requestResult = graphServiceClient.solutions().businessScenariosById('businessScenario-id').patch(requestBody);


```