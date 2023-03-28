---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnifiedRoleAssignmentMultiple();
$requestBody.setDisplayName('NewName');

$requestBody.setDescription('A new roleAssignment');



$requestResult = $graphServiceClient.roleManagement().cloudPC().roleAssignmentsById('unifiedRoleAssignmentMultiple-id').patch($requestBody);


```