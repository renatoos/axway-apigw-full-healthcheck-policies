# axway-apigw-full-healthcheck-policies


This project describes how to perform a full components healthcheck plus a zero downtime policy deployment to Axway API Gateway in a multi-node environment with a load balancer.

Contents
1.	Heathcheck APIGW Architecture	3
2.	Introduction to Zero Downtime Deploy	4
3.	Introduction to Virtualized Healthcheck	5
4.	Create the CassandraHC Policy	6
Create a new policy CassandraHC and organize the filters as the image below.	7
Edit the “Read Organization” filter to search the Community organization from API Portal.	7
Edit the “Set Message” filter to create the Cassandra error message.	7
Edit the “Reflect Message” filter  Create a Policy shortcut to HealthcheckLB.	8
Create a relative path to expose the policy.	8
Deploy the configuration	8
5.	Create the Routing Policy	9
On Policy Studio, create the policy “Routing HealthcheckLB”	9
Set the policy to API Manager Routing policies	9
Deploy the configuration	9
6.	Virtualize the API	10
Register Backend API	10
Virtualize on Frontend	11
1.	Set the Inbound Security	11
2.	Set the outbound Configuration	11
3.	Save the API and set the API as Published	11
4.	Test the API	12
7.	Deploy Zero Downtime Configuration	13

