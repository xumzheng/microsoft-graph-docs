---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Deployment()
request_body.@odatatype = '#microsoft.graph.windowsUpdates.deployment'

state = DeploymentState()
state.@odatatype = 'microsoft.graph.windowsUpdates.deploymentState'

state.RequestedValue(RequestedDeploymentStateValue('paused'))


request_body.state = state


request_configuration = DeploymentRequestBuilderPatchRequestConfiguration(
)


result = await client.admin.windows.updates.deployments_by_id('deployment-id').patch(request_body = request_body)


```