# Spring Boot Web Application
This repository has the project files for a tutorial series on Spring Boot available from by website at [Spring Framework Guru](https://springframework.guru)

## Checkout the full tutorial here!
[Spring Boot - making Spring Fun again!](https://springframework.guru/spring-boot-web-application-part-1-spring-initializr/)


For Midas:
I think we can keep our existing repo names. If we want to move over only a subset, I would prioritize the first 3.

1.	eb-services
2.	eb-ui
3.	eb-python-services
4.	eb-microservices
5.	eb-config
6.	eb-scripts (no pipeline needed)
7.	eb-plan-designs (no pipeline needed)
8.	eb-rating-engine (no pipeline needed)

Pipelines:
1.	eb-services
a.	mds-batch
b.	eb-benefit-admin
c.	eb-broker-agent
d.	mds-data
e.	eb-document
f.	eb-employer
g.	eb-gateway
h.	eb-lookup
i.	eb-messaging
j.	eb-nbo
k.	eb-people
l.	eb-plan
m.	eb-policy-enrollment
n.	eb-public-api
o.	eb-rfp
p.	eb-scheduling
q.	eb-security (build only, no release pipeline)
r.	eb-shared (build only, no release pipeline)
s.	eb-stonebranch
t.	eb-workflow
2.	eb-ui
a.	eb-sage
b.	eb-midas
c.	eb-eoi
d.	eb-par3
e.	eb-par
f.	eb-public-ui
3.	eb-python-services (just 1 pipeline, same name)
4.	eb-microservices (No pipelines needed: we are hoping to sunset this by end of 2023, so I think we can move the code to take advantage of CoPilot but not move the pipelines)
5.	eb-config (No pipeline needed at this time – I think we may be able to get rid of this one eventually)
