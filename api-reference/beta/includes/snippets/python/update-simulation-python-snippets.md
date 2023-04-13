---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Simulation()
request_body.displayName = 'Graph Simulation'

request_body.duration_in_days = 7

request_body.AttackTechnique(SimulationAttackTechnique('credentialharvesting'))

request_body.AttackType(SimulationAttackType('social'))

request_body.Status(SimulationStatus('scheduled'))

included_account_target = AccountTargetContent()
includedAccountTarget.@odatatype = '#microsoft.graph.addressBookAccountTargetContent'

includedAccountTarget.Type(AccountTargetContentType('addressbook'))

additionalData = [
'accountTargetEmails' => ['faiza@contoso.com', ],
];
includedAccountTarget.additionaldata(additionalData)



request_body.included_account_target = includedAccountTarget
excluded_account_target = AccountTargetContent()
excludedAccountTarget.@odatatype = '#microsoft.graph.addressBookAccountTargetContent'

excludedAccountTarget.Type(AccountTargetContentType('addressbook'))

additionalData = [
'accountTargetEmails' => ['sam@contoso.com', ],
];
excludedAccountTarget.additionaldata(additionalData)



request_body.excluded_account_target = excludedAccountTarget
additionalData = [
'@odata.etag' => '\"0100aa9b-0000-0100-0000-6396fa270000\"', 
'payload@odata.bind' => 'https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a', 
];
request_body.additionaldata(additionalData)





result = await client.security.attackSimulation.simulations_by_id('simulation-id').patch(request_body = request_body)


```