---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Simulation();
$requestBody->setDisplayName('Graph Simulation');

$requestBody->setDurationInDays(7);

$requestBody->setAttackTechnique(new SimulationAttackTechnique('credentialharvesting'));

$requestBody->setStatus(new SimulationStatus('scheduled'));

$requestBody->setDurationInDays(3);

$includedAccountTarget = new AccountTargetContent();
$includedAccountTarget->set@odatatype('#microsoft.graph.addressBookAccountTargetContent');

$includedAccountTarget->setType(new AccountTargetContentType('addressbook'));

$additionalData = [
'accountTargetEmails' => ['john@contoso.com', ],
];
$includedAccountTarget->setAdditionalData($additionalData);



$requestBody->setIncludedAccountTarget($includedAccountTarget);
$additionalData = [
'payload@odata.bind' => 'https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->security()->attackSimulation()->simulations()->post($requestBody);


```