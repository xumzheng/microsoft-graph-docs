---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GovernanceRoleAssignmentRequest()
request_body.setRoleDefinitionId('bc75b4e6-7403-4243-bf2f-d1f6990be122')

request_body.setResourceId('fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735')

request_body.setSubjectId('918e54be-12c4-4f4c-a6d3-2ee0e3661c51')

request_body.setAssignmentState('Active')

request_body.setType('UserRemove')

request_body.setReason('Deactivate the role')

request_body.setLinkedEligibleRoleAssignmentId('cb8a533e-02d5-42ad-8499-916b1e4822ec')



result = await client.privilegedAccess_by_id('privilegedAccess-id').roleAssignmentRequests.post(request_body)


```