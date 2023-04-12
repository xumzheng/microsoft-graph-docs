---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Simulation()
request_body.id = '2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc'

request_body.displayName = 'Graph Simulation'

request_body.durationInDays = 7

request_body.AttackTechnique(SimulationAttackTechnique('credentialharvesting'))

request_body.AttackType(SimulationAttackType('social'))

request_body.Status(SimulationStatus('scheduled'))

includedAccountTarget = AccountTargetContent()
includedAccountTarget.@odatatype = '#microsoft.graph.addressBookAccountTargetContent'

includedAccountTarget.Type(AccountTargetContentType('addressbook'))

additionalData = [
'accountTargetEmails' => ['faiza@contoso.com', ],
];
includedAccountTarget.additionaldata(additionalData)



request_body.includedAccountTarget = includedAccountTarget
excludedAccountTarget = AccountTargetContent()
excludedAccountTarget.@odatatype = '#microsoft.graph.addressBookAccountTargetContent'

excludedAccountTarget.Type(AccountTargetContentType('addressbook'))

additionalData = [
'accountTargetEmails' => ['sam@contoso.com', ],
];
excludedAccountTarget.additionaldata(additionalData)



request_body.excludedAccountTarget = excludedAccountTarget
additionalData = [
'@odata.etag' => '\"0100aa9b-0000-0100-0000-6396fa270000\"', 
'payload@odata.bind' => 'https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a', 
];
request_body.additionaldata(additionalData)





result = await client.security.attackSimulation.simulations_by_id('simulation-id').patch(request_body = request_body)


```