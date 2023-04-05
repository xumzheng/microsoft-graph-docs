---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Contact()
homeAddress = PhysicalAddress()
homeAddress.setStreet('123 Some street')

homeAddress.setCity('Seattle')

homeAddress.setState('WA')

homeAddress.setPostalCode('98121')


request_body.setHomeAddress($homeAddress)
request_body.setBirthday(DateTime('1974-07-22'))



result = await client.me.contacts_by_id('contact-id').patch(request_body)


```