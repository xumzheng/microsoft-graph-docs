---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DelegatedAdminAccessAssignmentRequestBuilderDeleteRequestConfiguration();

headers = [
	'If-Match' => 'W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="',
];

requestConfiguration.headers = headers;


graphServiceClient.tenantRelationships().delegatedAdminRelationshipsById('delegatedAdminRelationship-id').accessAssignmentsById('delegatedAdminAccessAssignment-id').delete(requestConfiguration);


```