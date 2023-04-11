---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SubjectRightsRequest()
request_body.Type(SubjectRightsRequestType('subjectrightsrequesttype'))

request_body.DataSubjectType(DataSubjectType('datasubjecttype'))

request_body.Regulations(['String', ])

request_body.displayName = 'String'

request_body.description = 'String'

request_body.internalDueDateTime = DateTime('String (timestamp)')

dataSubject = DataSubject()
dataSubject.firstName = 'String'

dataSubject.lastName = 'String'

dataSubject.email = 'String'

dataSubject.residency = 'String'

additionalData = [
'phoneNumber' => 'String', 
'SSN' => 'String', 
];
dataSubject.additionaldata(additionalData)



request_body.dataSubject = dataSubject


request_configuration = SubjectRightsRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.privacy.subjectRightsRequests.post(request_body = request_body)


```