---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "A Policy With Questions"
	Description = ""
	AllowedTargetScope = "allMemberUsers"
	Expiration = @{
		Type = "noExpiration"
	}
	RequestorSettings = @{
		EnableTargetsToSelfAddAccess = "true"
		EnableTargetsToSelfUpdateAccess = "true"
		EnableTargetsToSelfRemoveAccess = "true"
	}
	RequestApprovalSettings = @{
		IsApprovalRequiredForAdd = "true"
		IsApprovalRequiredForUpdate = "true"
		Stages = @(
			@{
				DurationBeforeAutomaticDenial = "P7D"
				IsApproverJustificationRequired = "false"
				IsEscalationEnabled = "false"
				FallbackPrimaryApprovers = @(
				)
				EscalationApprovers = @(
				)
				FallbackEscalationApprovers = @(
				)
				PrimaryApprovers = @(
					@{
						"@odata.type" = "#microsoft.graph.singleUser"
						UserId = "08a551cb-575a-4343-b914-f6e42798bd20"
					}
				)
			}
		)
	}
	Questions = @(
		@{
			"@odata.type" = "#microsoft.graph.accessPackageMultipleChoiceQuestion"
			Sequence = "1"
			IsRequired = "true"
			IsAnswerEditable = "true"
			Text = "What country are you working from?"
			IsMultipleSelectionAllowed = "false"
			Choices = @(
				@{
					"@odata.type" = "microsoft.graph.accessPackageAnswerChoice"
					ActualValue = "KE"
					Text = "Kenya"
				}
				@{
					"@odata.type" = "microsoft.graph.accessPackageAnswerChoice"
					ActualValue = "US"
					Text = "United States"
				}
				@{
					"@odata.type" = "microsoft.graph.accessPackageAnswerChoice"
					ActualValue = "GY"
					Text = "Guyana"
				}
				@{
					"@odata.type" = "microsoft.graph.accessPackageAnswerChoice"
					ActualValue = "BD"
					Text = "Bangladesh"
				}
				@{
					"@odata.type" = "microsoft.graph.accessPackageAnswerChoice"
					ActualValue = "JP"
					Text = "Japan"
				}
			)
		}
		@{
			"@odata.type" = "#microsoft.graph.accessPackageTextInputQuestion"
			Sequence = "2"
			IsRequired = "true"
			IsAnswerEditable = "true"
			Text = "What do you do for work?"
			Localizations = @(
				@{
					LanguageCode = "fr-CA"
					Text = "Que fais-tu comme travail?"
				}
			)
			IsSingleLineQuestion = "false"
			RegexPattern = "[a-zA-Z]+[a-zA-Z\s]*"
		}
	)
	AccessPackage = @{
		Id = "977c7ff4-ef8f-4910-9d31-49048ddf3120"
	}
}

New-MgEntitlementManagementAssignmentPolicy -BodyParameter $params

```