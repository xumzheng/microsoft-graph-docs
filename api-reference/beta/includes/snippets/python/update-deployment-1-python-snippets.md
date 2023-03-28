---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Deployment();
$requestBody.set@odatatype('#microsoft.graph.windowsUpdates.deployment');

$state = new DeploymentState();
$state.set@odatatype('microsoft.graph.windowsUpdates.deploymentState');

$state.setRequestedValue(new RequestedDeploymentStateValue('paused'));


$requestBody.setState($state);


$requestResult = $graphServiceClient.admin().windows().updates().deploymentsById('deployment-id').patch($requestBody);


```