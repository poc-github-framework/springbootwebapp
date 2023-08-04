# Spring Boot Web Application
This repository has the project files for a tutorial series on Spring Boot available from by website at [Spring Framework Guru](https://springframework.guru)

## Checkout the full tutorial here!
[Spring Boot - making Spring Fun again!](https://springframework.guru/spring-boot-web-application-part-1-spring-initializr/)
https://equprod-my.sharepoint.com/:v:/g/personal/alex_rau_equitable_com/EXWc1rvqcbtMpdB8u2MXTfkBvAKctIrHcOINiotLrqY24w

https://nam12.safelinks.protection.outlook.com/ap/w-59584e83/?url=https%3A%2F%2Fequprod.sharepoint.com%2F%3Aw%3A%2Fr%2Fsites%2FUSArchitectureGuild2%2FShared%2520Documents%2FDevOps%2520Tools%2FOnboarding%2520to%2520Github.docx%3Fd%3Dwdf3e896edc9941828393bd351e2f7689%26csf%3D1%26web%3D1%26e%3DsHaET1&data=05%7C01%7Ckaruppusamy.k%40dxc.com%7Cdb116ab4bdb04e8f62d708db941d4b10%7C93f33571550f43cfb09fcd331338d086%7C0%7C0%7C638266626732690301%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&sdata=YKgwV84TzBE874s9W6Oucw%2BOBOhlYwgZJ8Wjj0d%2BJg8%3D&reserved=0

https://nam12.safelinks.protection.outlook.com/ap/p-59584e83/?url=https%3A%2F%2Fequprod.sharepoint.com%2F%3Ap%3A%2Fr%2Fsites%2FUSArchitectureGuild2%2FShared%2520Documents%2FDevOps%2520Tools%2FGithub%2520Kickoff%2520with%2520new%2520teams.pptx%3Fd%3Dw9dc07e2ca28d4496bebd39b5f6275763%26csf%3D1%26web%3D1%26e%3DdTUTDh&data=05%7C01%7Ckaruppusamy.k%40dxc.com%7Cdb116ab4bdb04e8f62d708db941d4b10%7C93f33571550f43cfb09fcd331338d086%7C0%7C0%7C638266626732690301%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&sdata=1Cpf8muQNcKiTtLGAUZmSUvsgNmTQGMqQl4aqW9mkqY%3D&reserved=0

*****************************************Test*****************************************
1. ADO PAT (with all access) and GitHub PAT (with all access).
2. GitHub CLI installed
3. To perform this migration activity, you will need to be an organization owner or require migrator role.

Steps:
1. Authorise your git:
	gh auth login
2. Export you Personal Access Tokens:
 	export ADO_PAT="<ADO_PAT>"
	export GH_PAT="<GH_PAT>"
2. Install the ADO2GH Plugin.
	gh extension install github/gh-ado2gh
3. Upgrade the plugin:
 	gh extension upgrade github/gh-ado2gh
4. To migrate a single repo:
	gh ado2gh migrate-repo --ado-org SOURCE --ado-team-project TEAM-PROJECT --ado-repo CURRENT-NAME --github-org DESTINATION --github-repo NEW-NAME
5. To migrate multiple repos:
   First you would need to generate the migration script(comment out the repositories which are not being migrated):
	gh ado2gh generate-script --ado-org SOURCE --github-org DESTINATION --output FILENAME	 
   Run the script you generated:
	./FILENAME  
