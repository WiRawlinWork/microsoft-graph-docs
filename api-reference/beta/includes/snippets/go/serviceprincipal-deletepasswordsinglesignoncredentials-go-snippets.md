---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphserviceprincipals "github.com/microsoftgraph/msgraph-beta-sdk-go/serviceprincipals"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphserviceprincipals.NewDeletePasswordSingleSignOnCredentialsPostRequestBody()
id := "5793aa3b-cca9-4794-679a240f8b58"
requestBody.SetId(&id) 

graphClient.ServicePrincipals().ByServicePrincipalId("servicePrincipal-id").DeletePasswordSingleSignOnCredentials().Post(context.Background(), requestBody, nil)


```