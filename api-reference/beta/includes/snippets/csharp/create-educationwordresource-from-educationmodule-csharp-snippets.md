---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationModuleResource
{
	Resource = new EducationWordResource
	{
		OdataType = "#microsoft.graph.educationWordResource",
		DisplayName = "test_word_file.docx",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"file" , new 
				{
					Odataid = "https://graph.microsoft.com/v1.0/drives/b!-Ik2sRPLDEWy_bR8l75jfeDcpXQcRKVOmcml10NQLQ1F2UVvTgEnTKi0GO59dbCL/items/01VANVJQ23DHK5BYNOKJCZOUJZJBOAOUZP",
				}
			},
		},
	},
};
var result = await graphClient.Education.Classes["{educationClass-id}"].Modules["{educationModule-id}"].Resources.PostAsync(requestBody);


```