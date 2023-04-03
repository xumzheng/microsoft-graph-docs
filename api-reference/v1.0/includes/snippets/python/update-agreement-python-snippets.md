---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Agreement();
requestBody.setDisplayName('All Contoso volunteers - Terms of use');

requestBody.setIsViewingBeforeAcceptanceRequired(true);



result = awaitclient.identityGovernance().termsOfUse().agreementsById('agreement-id').patch(requestBody);


```