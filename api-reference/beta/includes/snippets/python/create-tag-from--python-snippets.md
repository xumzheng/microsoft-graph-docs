---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Tag()
request_body.setDisplayName('Privileged')

request_body.setDescription('The document is privileged')

additionalData = [
'parent@odata.bind' => 'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3', 
];
request_body.setAdditionalData(additionalData)




result = await client.compliance.ediscovery.casesById('case-id').tags.post(request_body)


```