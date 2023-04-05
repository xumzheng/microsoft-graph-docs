---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SubjectRightsRequest()
request_body.setType(SubjectRightsRequestType('export'))

request_body.setContentQuery('((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))')

request_body.setDataSubjectType(DataSubjectType('customer'))

request_body.setExternalId('F53BF2DA-607D-412A-B568-FAA0F023AC0B')

request_body.setDisplayName('Export report for customer Id: 12345')

request_body.setDescription('This is a export request')

request_body.setIncludeAllVersions(false)

request_body.setIncludeAuthoredContent(true)

request_body.setInternalDueDateTime(DateTime('2022-07-20T22:42:28Z'))

dataSubject = DataSubject()
dataSubject.setFirstName('Diego')

dataSubject.setLastName('Siciliani')

dataSubject.setEmail('Diego.Siciliani@contoso.com')

dataSubject.setResidency('USA')


request_body.setDataSubject($dataSubject)
request_body.setMailboxLocations(null)

request_body.setPauseAfterEstimate(true)

request_body.setRegulations(['CCPA', ])

siteLocations = SubjectRightsRequestSiteLocation()
siteLocations.set@odatatype('microsoft.graph.subjectRightsRequestAllSiteLocation')


request_body.setSiteLocations($siteLocations)
approversUser1 = User()
approversUser1.setId('1B761ED2-AA7E-4D82-9CF5-C09D737B6167')


approversArray []= approversUser1;
request_body.setApprovers(approversArray)




result = await client.privacy.subjectRightsRequests.post(request_body)


```