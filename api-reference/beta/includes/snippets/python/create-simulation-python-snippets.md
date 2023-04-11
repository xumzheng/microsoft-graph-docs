---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Simulation()
request_body.displayName = 'Graph Simulation'

request_body.durationInDays = 7

request_body.AttackTechnique(SimulationAttackTechnique('credentialharvesting'))

request_body.Status(SimulationStatus('scheduled'))

request_body.durationInDays = 3

includedAccountTarget = AccountTargetContent()
includedAccountTarget.@odatatype = '#microsoft.graph.addressBookAccountTargetContent'

includedAccountTarget.Type(AccountTargetContentType('addressbook'))

additionalData = [
'accountTargetEmails' => ['john@contoso.com', ],
];
includedAccountTarget.additionaldata(additionalData)



request_body.includedAccountTarget = includedAccountTarget
additionalData = [
'payload@odata.bind' => 'https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a', 
];
request_body.additionaldata(additionalData)





result = await client.security.attackSimulation.simulations.post(request_body = request_body)


```