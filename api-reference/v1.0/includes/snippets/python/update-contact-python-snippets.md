---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Contact()
home_address = PhysicalAddress()
homeAddress.street = '123 Some street'

homeAddress.city = 'Seattle'

homeAddress.state = 'WA'

homeAddress.postalCode = '98121'


request_body.home_address = homeAddress
request_body.birthday = DateTime('1974-07-22')




result = await client.me.contacts_by_id('contact-id').patch(request_body = request_body)


```