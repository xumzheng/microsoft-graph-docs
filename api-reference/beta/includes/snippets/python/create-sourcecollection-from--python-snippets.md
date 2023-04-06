---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceCollection()
request_body.setDisplayName('Quarterly Financials search')

request_body.setContentQuery('subject:\'Quarterly Financials\'')

additionalData = [
'custodianSources@odata.bind' => ['https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735', ],
];
request_body.setAdditionalData(additionalData)




result = await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections.post(request_body, headers=)


```