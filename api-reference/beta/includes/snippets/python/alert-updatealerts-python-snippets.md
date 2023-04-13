---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAlertsPostRequestBody()
value_alert1 = Alert()
valueAlert1.assignedTo = 'String'

valueAlert1.closedDateTime = DateTime('String (timestamp)')

valueAlert1.Comments(['String', ])

value_alert1_feedback = AlertFeedback()
additionalData = [
'@odata.type' => 'microsoft.graph.alertFeedback', 
];
valueAlert1Feedback.additionaldata(additionalData)



valueAlert1.feedback = valueAlert1Feedback
valueAlert1.id = 'String (identifier)'

value_alert1_status = AlertStatus()
additionalData = [
'@odata.type' => 'microsoft.graph.alertStatus', 
];
valueAlert1Status.additionaldata(additionalData)



valueAlert1.status = valueAlert1Status
valueAlert1.Tags(['String', ])

value_alert1_vendor_information = SecurityVendorInformation()
valueAlert1VendorInformation.provider = 'String'

valueAlert1VendorInformation.vendor = 'String'


valueAlert1.vendor_information = valueAlert1VendorInformation

valueArray []= valueAlert1;
request_body.value(valueArray)





result = await client.security.alerts.updateAlerts.post(request_body = request_body)


```