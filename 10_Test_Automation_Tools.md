## TEST AUTOMATION TOOLS

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

This chapter addresses different cost parameters to be aware of before procuring test automation tools for your organisation and briefly covers some of the widely used tools in functional testing, non-functional testing and test management. The demand for new automated testing tools keeps on changing with technology evolution, development approaches and market changes. The tool vendors continually deliver new tools to meet the market demand, and as such, it is difficult to list down and maintain a set of the latest tools at any point in time. The second part of this chapter lists a set of widely used tools for you to familiarise yourself with. This is not a recommendation of any tools over others or an endorsement of tool features.

Many organisations procure test automation tools without proper research, not understanding the licence model, professional support required or availability of in-house technical expertise and, as a result, end up disappointed. The tools themselves are often blamed after money and effort have been spent. Tool vendors often use terms such as ‘seat licence’, ‘concurrent licence’, ‘shared licence’, ‘annual licence’ or ‘professional service’, with costs associated with each. It is confusing and difficult to understand and decide on what is required and fit for purpose within an optimised cost. Many open-source tools have hidden costs such as add-ons or third-party solutions for features such as reporting and analysis.

The procurement process can be painful and time-consuming when the test automation manager drives it. Many organisations have a procurement process and team to assist the test automation team in gathering the information and procuring the tool on their behalf. Setting up and approving a new tool vendor takes time and a lot of follow-up, especially in big organisations. Also in many cases, the licence renewal process starts months before the licences expire.

The first part of this chapter describes different licence models, one of the major cost factors in most of the test automation activity. The second part introduces popular and common test automation tools available in the market. The third part of the chapter explains different cost factors to be considered for overall test automation tool costs.

10.1 UNDERSTANDING LICENCE MODELS

This section is intended to explain various licensing models and costs involved in procuring tools.

Firstly, some common terminologies related to tool licence management may be useful:

Software licence manager. This is a management tool used to control where and how software products are used. Licence managers protect, comply, monitor and track software licence agreements and usages. Licence managers offer a wide range of licensing models, such as product activation, trial licence, subscription licence, feature-based licence and floating licence. In many cases, the licence manager checks if the licence is in place remotely through the internet and tracks usage of the software. This tool is generally created by a vendor for their product or a bundle of products.

Software asset management or log. This is used by end-users to manage the software they have procured or licensed from many different software vendors. These are used to reconcile software licences and are largely managed on a spreadsheet for most small organisations. Large and medium size organisations maintain a **‘configuration management database’ or ‘CMDB repository’** that acts as a data warehouse for asset management. The CMDB stores information about the IT environment, the components, hardware assets, software assets (referred to as configuration items) and the licences.

Product activation. This is a licence validation mechanism, and it prevents the violation of the software licence. Activation allows the software to stop blocking features from the user when they move from using its free version to purchasing a licence.

Product key. This checks and confirms that the software is original from the vendor. For example, a physical copy of Microsoft Windows comes with a 25-character product key on a label or card inside the box, or the performance testing tool LoadRunner licence key can be downloaded online for an existing customer.

The list below covers different types of licence models and associated costs, often used in test automation tools:

- Public domain. These tools are available in the public domain and there is no ownership such as copyright, trademark or patents used to modify and distribute them. They are free to use.
- Licence-free. These tools are intended for free use, modification and distribution as long as the copyright is retained by the original owner.
- Free and open-source software (FOSS). These tools are freely licensed to use, and the source code is encouraged to be shared voluntarily with the community to improve the software. A few examples of FOSS are: Selenium, Appium, Apache JMeter, SoapUI and TestNG.
- Original equipment manufacturer (OEM). An OEM licence is generally installed by the manufacturer on new devices that are not usable on other machines, for example Microsoft Windows and anti-virus software are pre-installed on new Windows laptops. This licence is generally available for a short period unless renewed. Another example is the many browsers such as Chrome, Edge, Firefox and Safari that are pre-installed with compatibility and accessibility testing tools.
- General Public Licence (GPL). This is a free licence for end-users to learn, share and modify the software.
- Multi-licence. These distribute software under two or more different sets of terms and conditions, for example the software vendor distributes the same software to two different sets of end-users as GPL and OEM. The features of the software are the same. However, the usage is different.
- Permissive software licence. A free software licence with minimal restrictions of usage, modification and distribution.
- Proprietary software. This is under strict copyright licensing, and the source code is usually hidden from the end-users preventing modification, for example, Tosca and Eggplant.
- Subscription licence. This is a periodic renewable licence, for example users of Azure DevOps can either pay month-to-month through Azure or buy classic software licences, which require a 3-year commitment. BlazeMeter is another tool based on an annual subscription.
- Concurrent/floating licence. A software licence that is based on the number of simultaneous users accessing it. The software licence manager generally tracks and monitors the usage, and any user beyond the maximum concurrency is prohibited.
- Fixed licence. This is specific for a single machine, also known as a seat, and is used by a single user at any given time.
- Named licence. This is a single licence assigned to an individual user.
- Virtual users (VUs). This is generally a defined number of virtual users or ‘Vusers’ that can use the tool an unlimited number of times within a period. This is commonly used for performance testing tools.
- Pay-as-you-go licence. This is a licence based on usage.

The below figure represents the different licence models widely used in the IT industry.

Software licences are charged and managed these days smartly to provide maximum benefit to the tool users. However, it is important to understand the details of the terms and conditions before procuring the tool. It is strongly recommended to talk to the tool vendors and explore how the licence works as well as the infrastructure and professional support required prior to procurement.

Figure 10.1 Software licence models

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig10-1.png)

Software licensing is sometimes difficult to fully understand. There are various models used for licence costing and short-term and long-term costs involved. Infrastructure cost is another area to be considered during the costing process. A separate stand-alone licence manager is required to manage the licence in some cases.

Here’s an example from the industry:

A leading product development company required a performance and volume testing tool for their DevOps. The tool was expected to be used for daily testing, as well as a final round of full testing. Without a detailed understanding of it, they procured a tool with sufficient virtual users. However, they soon realised that the virtual users were not assigned periodically. The virtual users are charged in a ‘pay-as-you-go’ manner, that is, once you use a virtual user for a test the overall list is reduced. For example, if you procured 1000 virtual users for a month and used 1000 for your first test, you would end up with no virtual users for any further testing. This was different from the tool licence for many other tools that were widely available. The key message gained from this was that you should thoroughly understand the licence model before procuring a tool. The company decided to procure a different tool based on monthly subscription, with an unlimited number of virtual users for the remaining performance testing cycles.

10.2 LEADING TEST AUTOMATION TOOLS

This section lists testing categories, types and tools widely considered for test automation. Some of these tools are used for more than one type of testing. For example, Selenium can be used for web testing, functional testing, API testing and so on. There are many more tools and testing categories, such as accessibility testing, that are available in addition to those in the list below, which represents the common and leading testing tools:

- API/web services testing
- Unit testing
- Functional and web testing
- Mobile testing
- Test and defect management
- Cross-browser testing
- Performance and load testing
- Security testing
- AI and ML-powered testing tools
- Test framework tools

Figure 10.2 Testing tools

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig10-2.png)

The tables in this section cover a set of leading test automation tools and their key features that are used in the market for testing the categories listed above. There are many more tools available beyond this list, and it is recommended to perform a detailed comparison based on your needs before tool procurement. This section is not a recommendation of any tools over others or an endorsement of tool features.

10.2.1 API/web service testing tools

The below table covers a set of widely used API/web service test automation tools, and their key features.

Table 10.1 API/web service testing tools

|                |                                                                                                                                                                                                                                                                                                                                                                                                                             |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools          | Key features                                                                                                                                                                                                                                                                                                                                                                                                                |
| SoapUI         | Widely used for REST, SOAP, web service and API testingSupports record, edit and playback of HTTP communicationsEase of use including ‘drag and drop’ and integration with other toolsAllows the development of your own set of features as SoapUI pluginsHighly secure and open sourceUsed for automated functional, regression, security, API and load testing of web servicesSupports leading technologies and standards |
| Postman        | Popular API testing toolRuns on Windows, Mac and LinuxFacilitates collaboration and sharing of API dataAllows writing Boolean tests within Postman interface                                                                                                                                                                                                                                                                |
| REST Assured   | Framework to test REST servicesOpen-source platform with Java domain-specific languageGood community support                                                                                                                                                                                                                                                                                                                |
| RapidAPI       | Widely used with a large community baseTests wide variety of APIsUsed for functional and performance testing of web servicesIntegrates with CI/CD tools                                                                                                                                                                                                                                                                     |
| Katalon Studio | Supports SOAP and RESTful requestsUsed for API/web services, UI functional and mobile testingSupports data-driven approach                                                                                                                                                                                                                                                                                                  |

10.2.2 Unit testing tools

The below table covers a set of widely used unit test automation tools, and their key features.

Table 10.2 Unit testing tools

|          |                                                                                                                                                                                                                                   |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools    | Key features                                                                                                                                                                                                                      |
| JUnit    | Open-source unit testing frameworkSupports TDD environmentSpecifically designed for Java programmingWidely used and popular                                                                                                       |
| NUnit    | The unit testing framework is based on .NETSupports data-driven tests that can run in parallelPopular, and large user community                                                                                                   |
| TestNG   | Open-source test automation framework for Java programmingResembles JUnit and NUnitSupports concurrent and data-driven testingWidely used for functional and integration testing                                                  |
| HtmlUnit | An open-source unit testing framework that supports JavaScriptFramework for testing web applicationsIt provides GUI features such as forms, links and tablesOffers an open-source Java librarySupports protocols like HTTP, HTTPS |

10.2.3 Functional and web testing tools

The below table covers a set of widely used functional and web test automation tools and their key features.

10.2.4 Mobile testing

The below table covers a set of widely used mobile and tablet test automation tools, and their key features.

Table 10.3 Functional and web tools

|             |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools       | Key features                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Selenium    | Open-source functional testing toolPopular and widely usedUsed for web application testingAccepts test scripts in a variety of languages such as C#, Java, Perl, PHP, Python, Ruby and GroovyGood community supportCompatible with various browsers, Windows, Mac and LinuxProvides record and playback featuresIntegrates with Agile, DevOps and CD workflowsIntegrates with Selenium Grid, which allows cloud-based cross-browser testing using tools such as BrowserStack and SauceLabsSupports mobile testingA large set of libraries of plugins availableProvides cross-browser, cross-platform and third-party integrationsSupports parallel test execution |
| UFT One/QTP | Leading functional and web automation toolIt is licensed softwareSupports Java, .Net, SAP, Oracle, web servicesSupports mobile testing, cross-browser and third-party integrationsSupports data-driven and keyword-driven testsSupports leading test management tools                                                                                                                                                                                                                                                                                                                                                                                             |
| Tosca       | End-to-end functional and web testing toolUses a model-based approachIndependent of software technologiesUsed for functional and mobile testingProvides dashboards, analytics, integrations and distributed executionsSupports continuous integration and DevOps practicesRequires minimal technical knowledge                                                                                                                                                                                                                                                                                                                                                    |
| Eggplant    | A popular tool for functional, web and mobile testingTest cases can run from the command lineSupports Windows, macOS, iOS and Android                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |

Table 10.4 Mobile testing tools

|              |                                                                                                                                                                                                                                                                                                                                                                                    |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools        | Key features                                                                                                                                                                                                                                                                                                                                                                       |
| Appium       | Open-source test automation toolMobile testing tool for hybrid, native and web-based applicationsIt supports cross-platform and works on Mac and WindowsCreates UI tests and supports code reuseSupports test scripts across multiple programming languages, e.g. Java, Python, Ruby, JavaScript, PHPIntegrates with CI/CD toolsIntegrates with various frameworks and other tools |
| TestComplete | Provides UI tests for web, desktop and mobile applicationsAllows testing both native and hybrid mobile appsIt supports testing on multiple mobile platformsSupports JavaScript, Python, JScript, C# and C++Integrates with various CI/CD toolsOffers a record and playback feature and supports keyword-driven testsBuilt on top of the Appium open-source framework               |
| Robotium     | Open-source library designed specifically for Android UI testingSupports native and hybrid applicationsIntegrates with CI/CD toolsIntegrates with various frameworks and other tools                                                                                                                                                                                               |
| Kobiton      | Widely used for mobile testingSupports AppiumIntegrates with CI/CD toolsIntegrates with various frameworks and other tools                                                                                                                                                                                                                                                         |

10.2.5 Test management and defect management tools

Test management tools provide features to manage the end-to-end testing life cycle and process. Defect or bug management tools facilitate reporting, tracking, monitoring, closure and metrics of defects and bugs. A suite of test management, defect management, functional test automation and non-functional test automation tools from the same vendor is highly recommended as this helps in data flow across tools, providing a more accurate picture of the quality status, detailed reporting and single centralised licence management. These tools play an important role in test automation as they help to run the tests in a centralised manner, either on a scheduled nightly build or on a continuous integration build.

The below table provides a limited set of tools for reference. There is a wide variety of open-source and licensed tools available to cater to test management and defect management needs.

Table 10.5 Test and defect management tools

|              |                                                                                                                                                                                                                                                                                                                |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools        | Key features                                                                                                                                                                                                                                                                                                   |
| ALM          | Micro Focus Application Lifecycle Management (ALM) provides features for requirements management, test planning, test case development, test execution and defect managementPopular with Waterfall projectsWeb-based toolWidely used for test and defect managementAvailable in on-premises and cloud versions |
| Azure DevOps | Provides version control, requirements management, automated builds, testing, reporting and release managementPopular with Agile and DevOps projectsWidely used for defect managementWeb-based tool and available in on-premises and cloud versions                                                            |
| Jira         | Provides features for test, requirement, defect, reporting and release managementMany of the testing features come from add-on products from third parties with an additional licence feeWeb-based tool and popular with Agile and Kanban projects                                                             |

10.2.6 Cross-browser testing tools

Cross-browser testing tools provide features to test web applications on multiple browsers in a short span of time. This is known as browser compatibility testing and validates the solution across Chrome, Firefox, Internet Explorer (IE), Edge, Safari and other browsers.

The below table covers a set of widely used cross-browser testing tools, and their key features.

10.2.7 Performance and load testing tools

The below table covers a set of widely used performance, volume and load testing tools and their key features.

Table 10.6 Cross-browser testing tools

|              |                                                                                                                                                                                                                          |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Tools        | Key features                                                                                                                                                                                                             |
| LamdaTest    | Cloud-based cross-browser testing platformSupports manual, visual and automated testingValidates cross-browser testing on desktop and mobile browsers                                                                    |
| BrowserStack | Supports over 2000 different real browsers and devices versionsProvides features to validate cross-browser and operating system testing of web solutionsSupports CI/CDSupports Windows, Android, iOS and macOS platforms |
| Browsera     | Validates cross-browser layouts and scripting errors for web solutionsProvides automated browser compatibility testingSite crawling feature allows testing of all web pages on a single site                             |

Table 10.7 Performance and load testing tools

|                |                                                                                                                                                                                                                  |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools          | Key features                                                                                                                                                                                                     |
| LoadRunner     | Widely used and popular toolLicence-based testing tool for load testingLarge user community availableCompatible with Windows and LinuxWorks on several enterprise environmentsSupports several types of protocol |
| JMeter         | Open-source tool for load testingWidely used with a large user communitySupports various server types                                                                                                            |
| BlazeMeter     | Widely used for load testing of mobile apps, websites and APIsLicence-based tool for load testing                                                                                                                |
| Silk Performer | Licence-based testing tool for load testingLarge user community available                                                                                                                                        |

10.2.8 Security and penetration testing tools

The below table covers a set of widely used security, vulnerability and penetration testing tools and their key features.

Table 10.8 Security and penetration testing tools

|            |                                                                                                                                                                                                                                                                  |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools      | Key features                                                                                                                                                                                                                                                     |
| Netsparker | Security testing tool to check vulnerabilities in web applicationsPopular and widely used penetration testing toolSearches for exploitable SQL and cross-site scripting (XSS) vulnerabilities in web applicationsValidates cross-site scripting to SQL injection |
| Acunetix   | Security testing tool to check vulnerabilities in web applicationsWidely used penetration testing toolValidates cross-site scripting testing and in-depth SQL injectionProvides on-premises and cloud testing solution                                           |

10.2.9 AI/ML powered testing tools

AI and ML-powered testing tools predict where quality issues are most likely to occur, correlate data, and quickly identify and resolve issues accordingly.

The below table covers a set of widely used AI/ML testing tools and their key features.

Table 10.9 AL/ML powered testing tools

|                |                                                                                                                                                                          |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Tools          | Key features                                                                                                                                                             |
| Applitools SDK | Supports all major test automation frameworks and programming languages covering web, mobile and desktop appsIntegrates with GitHub, Microsoft Azure, DevOps etc.        |
| Eggplant AI    | Uses model-based approach to auto-generate test casesIncreases test coverage by designing test cases-based user behaviour                                                |
| Retest         | Automatically automates testsDetects functional differences and visual differences                                                                                       |
| Mabl           | Provides features for test generation and executionProvides scriptless tests, cross-browser testing and adaptive auto-healingMeasures the performance of the application |

10.2.10 Test framework tools

There is another set of tools under the wider category ‘test framework tools’ that are frequently used by the business users and non-technical testers in test automation effort. These enable data-driven testing and keyword-driven testing much more than single test automation tools or libraries. This list includes test frameworks in general that can call other libraries and tools. This category includes tools targeted to support BDD and ATDD approaches.

The below table covers a set of widely used tools to support business users and non-technical testers, and their key features.

Table 10.10 Test framework tools

|          |                                                                                                                                                            |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools    | Key features                                                                                                                                               |
| Cucumber | Widely used for BDDAvailable for most mainstream programming languagesUses business facing documentation and is used for ATDD                              |
| JBehave  | A framework for BDDSupports ATDD                                                                                                                           |
| Behat    | An open-source BDD framework for PHPEnables communication between developers, business and testersTest scenarios are written using Gherkin                 |
| Fitnesse | Supports ATDDWidely used to collaborate with business usersOpen-source tool used for web/GUI tests                                                         |
| Serenity | Widely used for ATDD and regression testsIntegrates with BDD and REST Assured for API testingWorks as a wrapper on top of Selenium WebDriver and BDD tools |

10.3 COST FACTORS

Cost is a key factor in test automation and test automation tool setup. It is important to understand the various costs involved in tool procurement, licence model, annual maintenance, professional services and, most importantly, the infrastructure required to set up test automation tools. Below is a list of cost factors to be considered and explored further during the tool set-up stages:

- Tool infrastructure and setup – Open-source and licensed automation tools setup involves infrastructure costs. Performance testing involves high infrastructure cost and a large volume of virtual users. Client, server, database, reporting and storing need to be considered.
- SaaS, PaaS and hybrid – Cloud and on-premises versions of the tools involve different costs. A cloud-based version involves enabling access to the cloud and configuring the test environment to the SaaS/PaaS platform. This may involve changing the firewall, load balancer configuration, network changes, adding Internet Protocol (IP) addresses to the white list and so on. The security aspects should be considered while accessing the cloud-based testing tools. All the above factors need to be considered for estimating the effort and cost.
- On-premises – On-premises and stand-alone secure environments require additional cost to download the tool to a separate media and physically install the tool to the environment. The test team may require special privileges and access to the environment to deploy the tool. This involves building and accessing the physical or virtual infrastructure. The time to coordinate with the vendor, infrastructure team, scheduling the downtime to do the upgrade, rolling back if something goes wrong and so on all need to be considered.
- Detailed design – An automation tool is another software application in the environment, and any tool in the environment may require a detailed design and approval from the engineering team before installation and deployment. Sometimes it requires a change board to approve the installation. This will involve additional effort from the test team and other teams such as technical architects or change management.
- Procurement – In a consulting or SI environment, it is recommended to procure the automation tool through the SI as they have good expertise in procuring tools for many customers and long-term partnerships with the tool partners. This helps to procure the tool at a considerably reduced rate. However, there is a service fee charged by the SI.
- Training – There is a learning cost involved for many tools, and tool vendors charge for training and installation support.
- Professional services – Ongoing support and maintenance from the tool vendor.
- Licence model – Understand how the licence costs work, for example a leading performance testing tool in the market has a ‘use and lose’ model as every load testing reduces the Vusers from the total numbers procured.
- Renewal – The renewal charge is another factor to be considered for tool selection and cost.

It is important to consider all the above cost factors before procuring the test automation tool. You may need to contact an existing tool user and the respective vendor to understand the costs involved in test automation tools.

10.4 SUMMARY

This chapter summarised licence models for tools, the most common and widely used tools available in the market at the time of writing and the cost involved in test automation tool setup. This is a key area in ROI calculation and tool selection. The next chapter further explores coding and programming languages used for test automation.
