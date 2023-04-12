---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AlertRule()
request_body.Severity(RuleSeverityType('informational'))

request_body.enabled = true

threshold = RuleThreshold()
threshold.Aggregation(AggregationType('count'))

threshold.Operator(OperatorType('greaterorequal'))

threshold.target = 90


request_body.threshold = threshold
notificationChannelsNotificationChannel1 = NotificationChannel()
notificationChannelsNotificationChannel1.NotificationChannelType(NotificationChannelType('portal'))

notificationChannelsNotificationChannel1.Receivers(['', ])

notificationChannelsNotificationChannel1.NotificationReceivers([])


notificationChannelsArray []= notificationChannelsNotificationChannel1;
notificationChannelsNotificationChannel2 = NotificationChannel()
notificationChannelsNotificationChannel2.NotificationChannelType(NotificationChannelType('email'))

notificationChannelsNotificationChannel2.Receivers(['serena.davis@contoso.com', ])

notificationReceiversNotificationReceiver1 = NotificationReceiver()
notificationReceiversNotificationReceiver1.locale = 'en-us'

notificationReceiversNotificationReceiver1.contactInformation = 'serena.davis@contoso.com'


notificationReceiversArray []= notificationReceiversNotificationReceiver1;
notificationChannelsNotificationChannel2.notificationreceivers(notificationReceiversArray)



notificationChannelsArray []= notificationChannelsNotificationChannel2;
request_body.notificationchannels(notificationChannelsArray)





result = await client.deviceManagement.monitoring.alertRules_by_id('alertRule-id').patch(request_body = request_body)


```