# Spring Boot Web Application --
This repository has the project files for a tutorial series on Spring Boot available from by website at [Spring Framework Guru](https://springframework.guru)

## Checkout the full tutorial here!
[Spring Boot - making Spring Fun again!](https://springframework.guru/spring-boot-web-application-part-1-spring-initializr/)
https://equprod-my.sharepoint.com/:v:/g/personal/alex_rau_equitable_com/EXWc1rvqcbtMpdB8u2MXTfkBvAKctIrHcOINiotLrqY24w

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
