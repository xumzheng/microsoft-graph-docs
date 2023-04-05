---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Deployment()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.deployment')

state = DeploymentState()
state.set@odatatype('microsoft.graph.windowsUpdates.deploymentState')

state.setRequestedValue(RequestedDeploymentStateValue('paused'))


request_body.setState($state)


result = await client.admin.windows.updates.deploymentsby_id('deployment-id').patch(request_body)


```