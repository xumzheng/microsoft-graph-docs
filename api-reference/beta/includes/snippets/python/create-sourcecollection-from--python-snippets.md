---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SourceCollection();
requestBody.setDisplayName('Quarterly Financials search');

requestBody.setContentQuery('subject:\'Quarterly Financials\'');

additionalData = [
'custodianSources@odata.bind' => ['https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735', ],
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.compliance().ediscovery().casesById('case-id').sourceCollections().post(requestBody);


```