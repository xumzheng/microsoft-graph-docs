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

requestBody.setAttackType(SimulationAttackType('social'));

requestBody.setStatus(SimulationStatus('scheduled'));

includedAccountTarget = AccountTargetContent();
includedAccountTarget.set@odatatype('#microsoft.graph.addressBookAccountTargetContent');

includedAccountTarget.setType(AccountTargetContentType('addressbook'));

additionalData = [
'accountTargetEmails' => ['faiza@contoso.com', ],
];
includedAccountTarget.setAdditionalData(additionalData);



requestBody.setIncludedAccountTarget($includedAccountTarget);
excludedAccountTarget = AccountTargetContent();
excludedAccountTarget.set@odatatype('#microsoft.graph.addressBookAccountTargetContent');

excludedAccountTarget.setType(AccountTargetContentType('addressbook'));

additionalData = [
'accountTargetEmails' => ['sam@contoso.com', ],
];
excludedAccountTarget.setAdditionalData(additionalData);



requestBody.setExcludedAccountTarget($excludedAccountTarget);
additionalData = [
'@odata.etag' => '\"0100aa9b-0000-0100-0000-6396fa270000\"', 
'payload@odata.bind' => 'https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a', 
];
requestBody.setAdditionalData(additionalData);




result = await client.security().attackSimulation().simulationsById('simulation-id').patch(requestBody);


```