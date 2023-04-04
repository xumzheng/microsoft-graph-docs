---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Simulation();
request_body.setDisplayName('Graph Simulation');

request_body.setDurationInDays(7);

request_body.setAttackTechnique(SimulationAttackTechnique('credentialharvesting'));

request_body.setStatus(SimulationStatus('scheduled'));

request_body.setDurationInDays(3);

includedAccountTarget = AccountTargetContent();
includedAccountTarget.set@odatatype('#microsoft.graph.addressBookAccountTargetContent');

includedAccountTarget.setType(AccountTargetContentType('addressbook'));

additionalData = [
'accountTargetEmails' => ['john@contoso.com', ],
];
includedAccountTarget.setAdditionalData(additionalData);



request_body.setIncludedAccountTarget($includedAccountTarget);
additionalData = [
'payload@odata.bind' => 'https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a', 
];
request_body.setAdditionalData(additionalData);




result = await client.security().attackSimulation().simulations().post(request_body);


```