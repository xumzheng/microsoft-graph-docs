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

residence_address = PhysicalAddress()
residenceAddress.@odatatype = 'microsoft.graph.physicalAddress'


request_body.residence_address = residenceAddress
mailing_address = PhysicalAddress()
mailingAddress.@odatatype = 'microsoft.graph.physicalAddress'


request_body.mailing_address = mailingAddress
student = EducationStudent()
student.@odatatype = 'microsoft.graph.educationStudent'


request_body.student = student
teacher = EducationTeacher()
teacher.@odatatype = 'microsoft.graph.educationTeacher'


request_body.teacher = teacher
created_by = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.created_by = createdBy
request_body.account_enabled = Boolean

assigned_licenses_assigned_license1 = AssignedLicense()
assignedLicensesAssignedLicense1.@odatatype = 'microsoft.graph.assignedLicense'


assignedLicensesArray []= assignedLicensesAssignedLicense1;
request_body.assignedlicenses(assignedLicensesArray)


assigned_plans_assigned_plan1 = AssignedPlan()
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

password_profile = PasswordProfile()
passwordProfile.@odatatype = 'microsoft.graph.passwordProfile'


request_body.password_profile = passwordProfile
request_body.officeLocation = 'String'

request_body.preferredLanguage = 'String'

provisioned_plans_provisioned_plan1 = ProvisionedPlan()
provisionedPlansProvisionedPlan1.@odatatype = 'microsoft.graph.provisionedPlan'


provisionedPlansArray []= provisionedPlansProvisionedPlan1;
request_body.provisionedplans(provisionedPlansArray)


request_body.refreshTokensValidFromDateTime = DateTime('String (timestamp)')

request_body.show_in_address_list = Boolean

request_body.surname = 'String'

request_body.usageLocation = 'String'

request_body.userPrincipalName = 'String'

request_body.userType = 'String'

on_premises_info = EducationOnPremisesInfo()
onPremisesInfo.@odatatype = 'microsoft.graph.educationOnPremisesInfo'


request_body.on_premises_info = onPremisesInfo



result = await client.education.users.post(request_body = request_body)


```