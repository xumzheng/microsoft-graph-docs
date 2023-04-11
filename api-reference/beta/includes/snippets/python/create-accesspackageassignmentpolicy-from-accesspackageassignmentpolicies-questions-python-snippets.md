---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.accessPackageId = 'b2eba9a1-b357-42ee-83a8-336522ed6cbf'

request_body.displayName = 'Users from connected organizations can request'

request_body.description = 'Allow users from configured connected organizations to request and be approved by their sponsors'

request_body.canExtend = false

request_body.durationInDays = 365

request_body.expirationDateTime=null

requestorSettings = RequestorSettings()
requestorSettings.scopeType = 'AllExistingConnectedOrganizationSubjects'

requestorSettings.acceptRequests = true


request_body.requestorSettings = requestorSettings
requestApprovalSettings = ApprovalSettings()
requestApprovalSettings.isApprovalRequired = true

requestApprovalSettings.isApprovalRequiredForExtension = false

requestApprovalSettings.isRequestorJustificationRequired = true

requestApprovalSettings.approvalMode = 'SingleStage'

approvalStagesApprovalStage1 = ApprovalStage()
approvalStagesApprovalStage1.approvalStageTimeOutInDays = 14

approvalStagesApprovalStage1.isApproverJustificationRequired = true

approvalStagesApprovalStage1.isEscalationEnabled = false

approvalStagesApprovalStage1.escalationTimeInMinutes = 11520

primaryApproversUserSet1 = UserSet()
primaryApproversUserSet1.@odatatype = '#microsoft.graph.groupMembers'

primaryApproversUserSet1.isBackup = true

additionalData = [
'id' => 'd2dcb9a1-a445-42ee-83a8-476522ed6cbf', 
'description' => 'group for users from connected organizations which have no external sponsor', 
];
primaryApproversUserSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primaryApproversUserSet2 = UserSet()
primaryApproversUserSet2.@odatatype = '#microsoft.graph.externalSponsors'

primaryApproversUserSet2.isBackup = false


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage1.primaryapprovers(primaryApproversArray)



approvalStagesArray []= approvalStagesApprovalStage1;
requestApprovalSettings.approvalstages(approvalStagesArray)



request_body.requestApprovalSettings = requestApprovalSettings
questionsAccessPackageQuestion1 = AccessPackageQuestion()
questionsAccessPackageQuestion1.isRequired = false

questionsAccessPackageQuestion1Text = AccessPackageLocalizedContent()
questionsAccessPackageQuestion1Text.defaultText = 'what state are you from?'

localizedTextsAccessPackageLocalizedText1 = AccessPackageLocalizedText()
localizedTextsAccessPackageLocalizedText1.text = '¿De qué estado eres?'

localizedTextsAccessPackageLocalizedText1.languageCode = 'es'


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questionsAccessPackageQuestion1Text.localizedtexts(localizedTextsArray)



questionsAccessPackageQuestion1.text = questionsAccessPackageQuestion1Text
questionsAccessPackageQuestion1.@odatatype = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

additionalData = [
'choices' => choices1 = ()
choices1.actualValue = 'AZ'

choices1DisplayValue = DisplayValue()
localizedTexts1 = ()
localizedTexts1.text = 'Arizona'

localizedTexts1.languageCode = 'es'


localizedTextsArray []= localizedTexts1;
choices1DisplayValue.localizedtexts(localizedTextsArray)



choices1.displayValue = choices1DisplayValue

choicesArray []= choices1;
choices2 = ()
choices2.actualValue = 'CA'

choices2DisplayValue = DisplayValue()
localizedTexts1 = ()
localizedTexts1.text = 'California'

localizedTexts1.languageCode = 'es'


localizedTextsArray []= localizedTexts1;
choices2DisplayValue.localizedtexts(localizedTextsArray)



choices2.displayValue = choices2DisplayValue

choicesArray []= choices2;
choices3 = ()
choices3.actualValue = 'OH'

choices3DisplayValue = DisplayValue()
localizedTexts1 = ()
localizedTexts1.text = 'Ohio'

localizedTexts1.languageCode = 'es'


localizedTextsArray []= localizedTexts1;
choices3DisplayValue.localizedtexts(localizedTextsArray)



choices3.displayValue = choices3DisplayValue

choicesArray []= choices3;
questionsAccessPackageQuestion1.choices(choicesArray)


'allowsMultipleSelection' => false,
];
questionsAccessPackageQuestion1.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion1;
questionsAccessPackageQuestion2 = AccessPackageQuestion()
questionsAccessPackageQuestion2.isRequired = false

questionsAccessPackageQuestion2Text = AccessPackageLocalizedContent()
questionsAccessPackageQuestion2Text.defaultText = 'Who is your manager?'

localizedTextsAccessPackageLocalizedText1 = AccessPackageLocalizedText()
localizedTextsAccessPackageLocalizedText1.text = 'por qué necesita acceso a este paquete'

localizedTextsAccessPackageLocalizedText1.languageCode = 'es'


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questionsAccessPackageQuestion2Text.localizedtexts(localizedTextsArray)



questionsAccessPackageQuestion2.text = questionsAccessPackageQuestion2Text
questionsAccessPackageQuestion2.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

additionalData = [
'isSingleLineQuestion' => false,
];
questionsAccessPackageQuestion2.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion2;
request_body.questions(questionsArray)




request_configuration = AccessPackageAssignmentPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```