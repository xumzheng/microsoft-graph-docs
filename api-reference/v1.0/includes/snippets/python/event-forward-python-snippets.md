---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ForwardPostRequestBody()
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.address = 'danas@contoso.onmicrosoft.com'

toRecipientsRecipient1EmailAddress.name = 'Dana Swope'


toRecipientsRecipient1.emailAddress = toRecipientsRecipient1EmailAddress

toRecipientsArray []= toRecipientsRecipient1;
request_body.torecipients(toRecipientsArray)


request_body.comment = 'Dana, hope you can make this meeting.'



request_configuration = ForwardRequestBuilderPostRequestConfiguration(
)


await client.me.events_by_id('event-id').forward.post(request_body = request_body)


```