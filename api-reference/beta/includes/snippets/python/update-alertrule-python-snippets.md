---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AlertRule();
requestBody.setSeverity(RuleSeverityType('informational'));

requestBody.setEnabled(true);

threshold = RuleThreshold();
threshold.setAggregation(AggregationType('count'));

threshold.setOperator(OperatorType('greaterorequal'));

threshold.setTarget(90);


requestBody.setThreshold($threshold);
notificationChannelsNotificationChannel1 = NotificationChannel();
notificationChannelsNotificationChannel1.setNotificationChannelType(NotificationChannelType('portal'));

notificationChannelsNotificationChannel1.setReceivers(['', ]);

notificationChannelsNotificationChannel1.setNotificationReceivers([]);


notificationChannelsArray []= notificationChannelsNotificationChannel1;
notificationChannelsNotificationChannel2 = NotificationChannel();
notificationChannelsNotificationChannel2.setNotificationChannelType(NotificationChannelType('email'));

notificationChannelsNotificationChannel2.setReceivers(['serena.davis@contoso.com', ]);

notificationReceiversNotificationReceiver1 = NotificationReceiver();
notificationReceiversNotificationReceiver1.setLocale('en-us');

notificationReceiversNotificationReceiver1.setContactInformation('serena.davis@contoso.com');


notificationReceiversArray []= notificationReceiversNotificationReceiver1;
notificationChannelsNotificationChannel2.setNotificationReceivers(notificationReceiversArray);



notificationChannelsArray []= notificationChannelsNotificationChannel2;
requestBody.setNotificationChannels(notificationChannelsArray);




result = await client.deviceManagement().monitoring().alertRulesById('alertRule-id').patch(requestBody);


```