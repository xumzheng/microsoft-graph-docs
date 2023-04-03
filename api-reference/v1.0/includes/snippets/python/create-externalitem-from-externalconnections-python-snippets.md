---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ExternalItem();
aclAcl1 = Acl();
aclAcl1.setType(AclType('user'));

aclAcl1.setValue('e811976d-83df-4cbd-8b9b-5215b18aa874');

aclAcl1.setAccessType(AccessType('grant'));


aclArray []= aclAcl1;
aclAcl2 = Acl();
aclAcl2.setType(AclType('externalgroup'));

aclAcl2.setValue('14m1b9c38qe647f6a');

aclAcl2.setAccessType(AccessType('deny'));


aclArray []= aclAcl2;
requestBody.setAcl(aclArray);


properties = Properties();
additionalData = [
'title' => 'Error in the payment gateway', 
'priority' => 1,
'assignee' => 'john@contoso.com', 
];
properties.setAdditionalData(additionalData);



requestBody.setProperties($properties);
content = ExternalItemContent();
content.setValue('Error in payment gateway...');

content.setType(ExternalItemContentType('text'));


requestBody.setContent($content);


requestResult = graphServiceClient.external().connectionsById('externalConnection-id').itemsById('externalItem-id').put(requestBody);


```