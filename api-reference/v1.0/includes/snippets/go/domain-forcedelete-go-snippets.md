---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphdomains "github.com/microsoftgraph/msgraph-sdk-go/domains"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphdomains.NewForceDeletePostRequestBody()
disableUserAccounts := true
requestBody.SetDisableUserAccounts(&disableUserAccounts) 

graphClient.Domains().ByDomainId("domain-id").ForceDelete().Post(context.Background(), requestBody, nil)


```