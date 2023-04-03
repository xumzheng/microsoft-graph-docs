---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = LegalHold();
requestBody.set@odatatype('#microsoft.graph.ediscovery.legalHold');

requestBody.setDescription('String');

createdBy = IdentitySet();
createdBy.set@odatatype('microsoft.graph.identitySet');


requestBody.setCreatedBy($createdBy);
requestBody.setIsEnabled(boolean);

requestBody.setStatus(LegalHoldStatus('string'));

requestBody.setContentQuery('String');

requestBody.setErrors(['String', ]);

requestBody.setDisplayName('String');



requestResult = graphServiceClient.compliance().ediscovery().casesById('case-id').legalHolds().post(requestBody);


```