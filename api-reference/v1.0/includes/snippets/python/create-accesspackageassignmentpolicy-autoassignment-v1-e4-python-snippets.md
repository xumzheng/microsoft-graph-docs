---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.displayName = 'A Policy With Questions'

request_body.description = ''

request_body.AllowedTargetScope(AllowedTargetScope('allmemberusers'))

expiration = ExpirationPattern()
expiration.Type(ExpirationPatternType('noexpiration'))


request_body.expiration = expiration
requestorSettings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enableTargetsToSelfAddAccess = true

requestorSettings.enableTargetsToSelfUpdateAccess = true

requestorSettings.enableTargetsToSelfRemoveAccess = true


request_body.requestorSettings = requestorSettings
requestApprovalSettings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.isApprovalRequiredForAdd = true

requestApprovalSettings.isApprovalRequiredForUpdate = true

stagesAccessPackageApprovalStage1 = AccessPackageApprovalStage()
stagesAccessPackageApprovalStage1.durationbeforeautomaticdenial =  \DateInterval('P7D')

stagesAccessPackageApprovalStage1.isApproverJustificationRequired = false

stagesAccessPackageApprovalStage1.isEscalationEnabled = false

stagesAccessPackageApprovalStage1.FallbackPrimaryApprovers([])

stagesAccessPackageApprovalStage1.EscalationApprovers([])

stagesAccessPackageApprovalStage1.FallbackEscalationApprovers([])

primaryApproversSubjectSet1 = SubjectSet()
primaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => '08a551cb-575a-4343-b914-f6e42798bd20', 
];
primaryApproversSubjectSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.primaryapprovers(primaryApproversArray)



stagesArray []= stagesAccessPackageApprovalStage1;
requestApprovalSettings.stages(stagesArray)



request_body.requestApprovalSettings = requestApprovalSettings
questionsAccessPackageQuestion1 = AccessPackageQuestion()
questionsAccessPackageQuestion1.@odatatype = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

questionsAccessPackageQuestion1.sequence = 1

questionsAccessPackageQuestion1.isRequired = true

questionsAccessPackageQuestion1.isAnswerEditable = true

questionsAccessPackageQuestion1.text = 'What country are you working from?'

additionalData = [
'isMultipleSelectionAllowed' => 'false', 
'choices' => choices1 = ()
choices1.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices1.actualValue = 'KE'

choices1.text = 'Kenya'


choicesArray []= choices1;
choices2 = ()
choices2.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices2.actualValue = 'US'

choices2.text = 'United States'


choicesArray []= choices2;
choices3 = ()
choices3.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices3.actualValue = 'GY'

choices3.text = 'Guyana'


choicesArray []= choices3;
choices4 = ()
choices4.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices4.actualValue = 'BD'

choices4.text = 'Bangladesh'


choicesArray []= choices4;
choices5 = ()
choices5.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices5.actualValue = 'JP'

choices5.text = 'Japan'


choicesArray []= choices5;
questionsAccessPackageQuestion1.choices(choicesArray)


];
questionsAccessPackageQuestion1.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion1;
questionsAccessPackageQuestion2 = AccessPackageQuestion()
questionsAccessPackageQuestion2.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

questionsAccessPackageQuestion2.sequence = 2

questionsAccessPackageQuestion2.isRequired = true

questionsAccessPackageQuestion2.isAnswerEditable = true

questionsAccessPackageQuestion2.text = 'What do you do for work?'

localizationsAccessPackageLocalizedText1 = AccessPackageLocalizedText()
localizationsAccessPackageLocalizedText1.languageCode = 'fr-CA'

localizationsAccessPackageLocalizedText1.text = 'Que fais-tu comme travail?'


localizationsArray []= localizationsAccessPackageLocalizedText1;
questionsAccessPackageQuestion2.localizations(localizationsArray)


additionalData = [
'isSingleLineQuestion' => 'false', 
'regexPattern' => '[a-zA-Z]+[a-zA-Z\s]*', 
];
questionsAccessPackageQuestion2.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion2;
request_body.questions(questionsArray)


accessPackage = AccessPackage()
accessPackage.id = '977c7ff4-ef8f-4910-9d31-49048ddf3120'


request_body.accessPackage = accessPackage



result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body = request_body)


```