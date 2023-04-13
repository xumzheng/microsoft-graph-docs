---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExternalItem()
acl_acl1 = Acl()
aclAcl1.Type(AclType('user'))

aclAcl1.value = 'e811976d-83df-4cbd-8b9b-5215b18aa874'

aclAcl1.AccessType(AccessType('grant'))


aclArray []= aclAcl1;
acl_acl2 = Acl()
aclAcl2.Type(AclType('externalgroup'))

aclAcl2.value = '14m1b9c38qe647f6a'

aclAcl2.AccessType(AccessType('deny'))


aclArray []= aclAcl2;
request_body.acl(aclArray)


properties = Properties()
additionalData = [
'title' => 'Error in the payment gateway', 
'priority' => 1,
'assignee' => 'john@contoso.com', 
];
properties.additionaldata(additionalData)



request_body.properties = properties
content = ExternalItemContent()
content.value = 'Error in payment gateway...'

content.Type(ExternalItemContentType('text'))


request_body.content = content



result = await client.external.connections_by_id('externalConnection-id').items_by_id('externalItem-id').put(request_body = request_body)


```