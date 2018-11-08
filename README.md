# PerformanceTesting

- I am thankful to **Mark Tomlinson** helping me learn below points from performance test prespective while starting from scratch.
 
## Understand requirements :[Work with Team]
- PM can use analytics/tracking services to identify the critical scenario for application
- Identify the critical scenarios for performance testing (performance test should be done only for critical scenarios to business and application - not all scenarios.)
- Identify the scenarios at user perspective from PM
- Identify what all services are consumed to completing above user scenario with help of Developers of applications
 
## What the performance number they are looking for after testing?
- What is baseline numbers  ?
- How much we as a team we can deviate on performance on each release ?
 
## Understand architecture of application
- How the data is flowing ?
- What are different server mobile apps is consuming ?
 
## Understand what kind of test you wanted to do
- Server side ?
- Client side ?
- 2G AND 3G, 4G, WIFI - network speeds on mobile, Do they want to test this kind of scenario  ?
 
## Identify size of data estimated in production database ?
 - The system must support 400 concurrent users – Why ?(This help us to understand what is the exact business requirement)
 
## Server placed at different Region 

## Environment :[Work with Team]
 - Have a replica of production environment
 - Exactly same configuration of Mobile app. Example : app server & database server .. etc based on your application – identify that server memory, CPU, networks etc and replicate same.)
 
## Test Data: [QA]
 
- Data size estimated in production environments:
- Understand the size of database in production environment [1 million, 50 thousand size of data]
- The size of data mentioned by PM will help us to create test data for same size for replica environment.
 
## Set the scripts and run test :[QA]
 
- How to perform server side and client side test ?
- Server Side - Performance test of the server side hitting the api endpoints the mobile calls.  Use this to get the maximum response times for each API call.
- Client Side - Mobile devices tests with the server side API calls mocked out so that they return instantly. This will give you an idea of how long it takes the mobile devices to render data returned by the server.
- Results : Add 1+2  together to get the worst case scenario. I would suggest doing 2 with the lowest spec mobile you need to support
 
## Monitoring :[QA]
 - Set monitors for all servers on your application: app server, database server [CPU, Memory, network ] as to identify any memory leaks etc during L & P test.
 
 