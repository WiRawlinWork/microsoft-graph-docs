---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



graphClient.Me().MailFolders().ByMailFolderId("mailFolder-id").MessageRules().ByMessageRuleId("messageRule-id").Delete(context.Background(), nil)


```