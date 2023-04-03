---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UpdateAlertsPostRequestBody();
valueAlert1 = Alert();
valueAlert1.setAssignedTo('String');

valueAlert1.setClosedDateTime(DateTime('String (timestamp)'));

valueAlert1.setComments(['String', ]);

valueAlert1Feedback = AlertFeedback();
additionalData = [
'@odata.type' => 'microsoft.graph.alertFeedback', 
];
valueAlert1Feedback.setAdditionalData(additionalData);



valueAlert1.setFeedback($valueAlert1Feedback);
valueAlert1.setId('String (identifier)');

valueAlert1Status = AlertStatus();
additionalData = [
'@odata.type' => 'microsoft.graph.alertStatus', 
];
valueAlert1Status.setAdditionalData(additionalData);



valueAlert1.setStatus($valueAlert1Status);
valueAlert1.setTags(['String', ]);

valueAlert1VendorInformation = SecurityVendorInformation();
valueAlert1VendorInformation.setProvider('String');

valueAlert1VendorInformation.setVendor('String');


valueAlert1.setVendorInformation($valueAlert1VendorInformation);

valueArray []= valueAlert1;
requestBody.setValue(valueArray);




requestResult = graphServiceClient.security().alerts().updateAlerts().post(requestBody);


```