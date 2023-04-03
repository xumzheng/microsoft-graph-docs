---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RoleAssignmentScheduleRequestsRequestBuilderGetRequestConfiguration();

queryParameters = RoleAssignmentScheduleRequestsRequestBuilderGetQueryParameters();
queryParameters.select = ["principalId","action","roleDefinitionId"];
queryParameters.expand = ["roleDefinition","activatedUsing","principal","targetSchedule"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.roleManagement().directory().roleAssignmentScheduleRequests().get(requestConfiguration);


```