---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExternalItem()
aclAcl1 = Acl()
aclAcl1.setType(AclType('user'))

aclAcl1.setValue('e811976d-83df-4cbd-8b9b-5215b18aa874')

aclAcl1.setAccessType(AccessType('grant'))


aclArray []= aclAcl1;
aclAcl2 = Acl()
aclAcl2.setType(AclType('externalgroup'))

aclAcl2.setValue('14m1b9c38qe647f6a')

aclAcl2.setAccessType(AccessType('deny'))


aclArray []= aclAcl2;
request_body.setAcl(aclArray)


properties = Properties()
additionalData = [
'title' => 'Error in the payment gateway', 
'priority' => 1,
'assignee' => 'john@contoso.com', 
];
properties.setAdditionalData(additionalData)



request_body.setProperties($properties)
content = ExternalItemContent()
content.setValue('Error in payment gateway...')

content.setType(ExternalItemContentType('text'))


request_body.setContent($content)


result = await client.external.connections_by_id('externalConnection-id').items_by_id('externalItem-id').put(request_body, headers=)


```