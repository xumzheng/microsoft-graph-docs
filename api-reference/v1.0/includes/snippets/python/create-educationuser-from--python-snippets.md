---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationUser()
request_body.@odatatype = '#microsoft.graph.educationUser'

request_body.PrimaryRole(EducationUserRole('string'))

request_body.middleName = 'String'

request_body.ExternalSource(EducationExternalSource('string'))

request_body.externalSourceDetail = 'String'

residenceAddress = PhysicalAddress()
residenceAddress.@odatatype = 'microsoft.graph.physicalAddress'


request_body.residenceAddress = residenceAddress
mailingAddress = PhysicalAddress()
mailingAddress.@odatatype = 'microsoft.graph.physicalAddress'


request_body.mailingAddress = mailingAddress
student = EducationStudent()
student.@odatatype = 'microsoft.graph.educationStudent'


request_body.student = student
teacher = EducationTeacher()
teacher.@odatatype = 'microsoft.graph.educationTeacher'


request_body.teacher = teacher
createdBy = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.createdBy = createdBy
request_body.accountEnabled = boolean

assignedLicensesAssignedLicense1 = AssignedLicense()
assignedLicensesAssignedLicense1.@odatatype = 'microsoft.graph.assignedLicense'


assignedLicensesArray []= assignedLicensesAssignedLicense1;
request_body.assignedlicenses(assignedLicensesArray)


assignedPlansAssignedPlan1 = AssignedPlan()
assignedPlansAssignedPlan1.@odatatype = 'microsoft.graph.assignedPlan'


assignedPlansArray []= assignedPlansAssignedPlan1;
request_body.assignedplans(assignedPlansArray)


request_body.BusinessPhones(['String', ])

request_body.department = 'String'

request_body.displayName = 'String'

request_body.givenName = 'String'

request_body.mail = 'String'

request_body.mailNickname = 'String'

request_body.mobilePhone = 'String'

request_body.passwordPolicies = 'String'

passwordProfile = PasswordProfile()
passwordProfile.@odatatype = 'microsoft.graph.passwordProfile'


request_body.passwordProfile = passwordProfile
request_body.officeLocation = 'String'

request_body.preferredLanguage = 'String'

provisionedPlansProvisionedPlan1 = ProvisionedPlan()
provisionedPlansProvisionedPlan1.@odatatype = 'microsoft.graph.provisionedPlan'


provisionedPlansArray []= provisionedPlansProvisionedPlan1;
request_body.provisionedplans(provisionedPlansArray)


request_body.refreshTokensValidFromDateTime = DateTime('String (timestamp)')

request_body.showInAddressList = boolean

request_body.surname = 'String'

request_body.usageLocation = 'String'

request_body.userPrincipalName = 'String'

request_body.userType = 'String'

onPremisesInfo = EducationOnPremisesInfo()
onPremisesInfo.@odatatype = 'microsoft.graph.educationOnPremisesInfo'


request_body.onPremisesInfo = onPremisesInfo


request_configuration = UsersRequestBuilderPostRequestConfiguration(
)


result = await client.education.users.post(request_body = request_body)


```