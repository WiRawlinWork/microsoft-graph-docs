---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteList -SiteId $siteId -ListId $listId -Property "name,lastModifiedDateTime" -ExpandProperty "columns(select=name,description),items)" 

```