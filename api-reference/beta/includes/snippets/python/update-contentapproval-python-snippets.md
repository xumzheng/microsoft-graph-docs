---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ComplianceChange();
$requestBody->set@odatatype('#microsoft.graph.windowsUpdates.contentApproval');

$requestBody->setIsRevoked(true);



$requestResult = $graphServiceClient->admin()->windows()->updates()->updatePoliciesById('updatePolicy-id')->complianceChangesById('complianceChange-id')->patch($requestBody);


```