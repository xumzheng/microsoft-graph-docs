---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AlertRule()
request_body.setSeverity(RuleSeverityType('informational'))

request_body.setEnabled(true)

threshold = RuleThreshold()
threshold.setAggregation(AggregationType('count'))

threshold.setOperator(OperatorType('greaterorequal'))

threshold.setTarget(90)


request_body.setThreshold($threshold)
notificationChannelsNotificationChannel1 = NotificationChannel()
notificationChannelsNotificationChannel1.setNotificationChannelType(NotificationChannelType('portal'))

notificationChannelsNotificationChannel1.setReceivers(['', ])

notificationChannelsNotificationChannel1.setNotificationReceivers([])


notificationChannelsArray []= notificationChannelsNotificationChannel1;
notificationChannelsNotificationChannel2 = NotificationChannel()
notificationChannelsNotificationChannel2.setNotificationChannelType(NotificationChannelType('email'))

notificationChannelsNotificationChannel2.setReceivers(['serena.davis@contoso.com', ])

notificationReceiversNotificationReceiver1 = NotificationReceiver()
notificationReceiversNotificationReceiver1.setLocale('en-us')

notificationReceiversNotificationReceiver1.setContactInformation('serena.davis@contoso.com')


notificationReceiversArray []= notificationReceiversNotificationReceiver1;
notificationChannelsNotificationChannel2.setNotificationReceivers(notificationReceiversArray)



notificationChannelsArray []= notificationChannelsNotificationChannel2;
request_body.setNotificationChannels(notificationChannelsArray)




result = await client.deviceManagement.monitoring.alertRulesby_id('alertRule-id').patch(request_body)


```