---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentPolicy = {
	displayName : "policy for external access requests",
	description : "policy for users from connected organizations to request access, with two stages of approval.",
	allowedTargetScope : AllowedTargetScope.AllConfiguredConnectedOrganizationUsers,
	specificAllowedTargets : [
	],
	expiration : {
		type : ExpirationPatternType.NoExpiration,
	},
	requestorSettings : {
		enableTargetsToSelfAddAccess : true,
		enableTargetsToSelfUpdateAccess : true,
		enableTargetsToSelfRemoveAccess : true,
		allowCustomAssignmentSchedule : false,
		enableOnBehalfRequestorsToAddAccess : false,
		enableOnBehalfRequestorsToUpdateAccess : false,
		enableOnBehalfRequestorsToRemoveAccess : false,
		onBehalfRequestors : [
		],
	},
	requestApprovalSettings : {
		isApprovalRequiredForAdd : true,
		isApprovalRequiredForUpdate : false,
		stages : [
			{
				durationBeforeAutomaticDenial : "P14D",
				isApproverJustificationRequired : false,
				isEscalationEnabled : false,
				durationBeforeEscalation : "PT0S",
				primaryApprovers : [
					{
						"@odata.type" : "#microsoft.graph.internalSponsors",
					},
				],
				fallbackPrimaryApprovers : [
					{
						"@odata.type" : "#microsoft.graph.singleUser",
						additionalData : {
							"userId" : "7deff43e-1f17-44ef-9e5f-d516b0ba11d4",
						},
					},
					{
						"@odata.type" : "#microsoft.graph.groupMembers",
						additionalData : {
							"groupId" : "1623f912-5e86-41c2-af47-39dd67582b66",
						},
					},
				],
				escalationApprovers : [
				],
				fallbackEscalationApprovers : [
				],
			},
			{
				durationBeforeAutomaticDenial : "P14D",
				isApproverJustificationRequired : false,
				isEscalationEnabled : false,
				durationBeforeEscalation : "PT0S",
				primaryApprovers : [
				],
				fallbackPrimaryApprovers : [
					{
						"@odata.type" : "#microsoft.graph.singleUser",
						additionalData : {
							"userId" : "46184453-e63b-4f20-86c2-c557ed5d5df9",
						},
					},
					{
						"@odata.type" : "#microsoft.graph.groupMembers",
						additionalData : {
							"groupId" : "1623f912-5e86-41c2-af47-39dd67582b66",
						},
					},
				],
				escalationApprovers : [
				],
				fallbackEscalationApprovers : [
				],
			},
		],
	},
	reviewSettings : {
		isEnabled : true,
		expirationBehavior : AccessReviewExpirationBehavior.KeepAccess,
		isRecommendationEnabled : true,
		isReviewerJustificationRequired : true,
		isSelfReview : false,
		schedule : {
			startDateTime : new Date("2022-07-02T06:59:59.998Z"),
			expiration : {
				duration : "P14D",
				type : ExpirationPatternType.AfterDuration,
			},
			recurrence : {
				pattern : {
					type : RecurrencePatternType.AbsoluteMonthly,
					interval : 3,
					month : 0,
					dayOfMonth : 0,
					daysOfWeek : [
					],
				},
				range : {
					type : RecurrenceRangeType.NoEnd,
					numberOfOccurrences : 0,
				},
			},
		},
		primaryReviewers : [
			{
				"@odata.type" : "#microsoft.graph.groupMembers",
				additionalData : {
					"groupId" : "1623f912-5e86-41c2-af47-39dd67582b66",
				},
			},
		],
		fallbackReviewers : [
		],
	},
	accessPackage : {
		id : "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.assignmentPolicies.post(requestBody);
}


```