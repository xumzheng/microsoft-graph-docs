---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Simulation();
requestBody.setDisplayName('Graph Simulation');

requestBody.setDurationInDays(7);

requestBody.setAttackTechnique(SimulationAttackTechnique('credentialharvesting'));

requestBody.setStatus(SimulationStatus('scheduled'));

requestBody.setDurationInDays(3);

includedAccountTarget = AccountTargetContent();
includedAccountTarget.set@odatatype('#microsoft.graph.addressBookAccountTargetContent');

includedAccountTarget.setType(AccountTargetContentType('addressbook'));

additionalData = [
'accountTargetEmails' => ['john@contoso.com', ],
];
includedAccountTarget.setAdditionalData(additionalData);



requestBody.setIncludedAccountTarget($includedAccountTarget);
additionalData = [
'payload@odata.bind' => 'https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a', 
];
requestBody.setAdditionalData(additionalData);




result = await client.security().attackSimulation().simulations().post(requestBody);


```