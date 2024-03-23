## AUTOMATION FRAMEWORK DESIGN AND DEVELOPMENT

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

This chapter is essential for test automation engineers, architects, project managers, Scrum masters and everyone involved in test automation framework design and development. This chapter explains how to approach a test automation framework by using a spreadsheet for data management. This framework is based on the philosophy of using libraries for validation and reporting.

A framework is defined as a set of rules and guidelines, such as best practices and coding standards, that can be followed in a systematic way that ensures the delivery of targeted results such as increased code reusability, higher portability and reduced script maintenance costs. The right framework needs to be selected based on an organisation’s current and future needs. The essential criteria for any automation framework are its scalability, maintainability, and code that can be quickly understood, easy to debug and rapidly developed.

The primary objective of the framework is to maximise reusability of common components and libraries while minimising maintenance of the framework and automated tests. The framework is expected to provide the following benefits:

- Reusability of functions and libraries
- Quick test execution and low learning curve
- Low maintenance of the overall framework and automated test scripts
- Repeatability of regression tests on different environments
- Quick enhancement of the framework with new features

One key aspect of the test automation framework is that it is designed and developed with the intention of future use. The framework should be ‘generic’, meaning that it should be compatible with more than one application and product.

The first part of this chapter explains some common components and terminologies used in any standard test automation framework. The latter part of the chapter explains how to design and build a test automation framework.

A test automation framework is a programming framework that includes a comprehensive set of guidelines, standards, software packages, and testing tools to provide a foundation structure for developing a test automation suite.

12.1 TEST AUTOMATION COMPONENTS’ DEFINITIONS

In this section, we explore the definitions of some common phrases, terms and activities in test automation and relating to test automation frameworks. The purpose of this section is to familiarise you with the common terminologies in test automation.

Table 12.1 Common definitions

|                          |                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term                     | Definition                                                                                                                                                                                                                                                                                                                                                        |
| Editor                   | An automated test script is a set of instructions created by the tool or manually created by a human to validate the SUT. Automated scripts can be written in either a programming language using an editor or created by a testing tool. Editing is modifying the scripts using an editor.                                                                       |
| Object repository        | An object repository is a collection of objects and properties taken from the SUT for a testing tool to recognise the corresponding elements.                                                                                                                                                                                                                     |
| Library                  | A programming library is a suite of helper functions that another program can make use of. This may include common functionality, subroutines, classes, values or type specifications.                                                                                                                                                                            |
| Classes                  | In object-oriented programming, a class is an extensible program for creating objects.                                                                                                                                                                                                                                                                            |
| Exception handling       | This is the process of a program responding to exceptions or unexpected behaviour.                                                                                                                                                                                                                                                                                |
| Recovery scenario        | This contains generic functions to handle exceptions at runtime.                                                                                                                                                                                                                                                                                                  |
| GUI objects              | An object has a state (data) and behaviour (code) and is an abstract data type with the addition of polymorphism and inheritance. GUI objects are the same, representing GUI elements such as text boxes, buttons and check boxes.                                                                                                                                |
| Configuration management | Configuration management is the tracking and controlling of changes in software including version control. Configuration management is essential to maintain software, system and document integrity and consistency once the solution has been developed and released by multiple teams or in multiple environments across a wide range of end-user communities. |
| Deployment               | Software deployment is the process of making the application available on a target place: test server, production environment, mobile device etc.                                                                                                                                                                                                                 |
| Test automation script   | A test automation script is a set of instructions that will be performed on the SUT to validate that it works as expected. Good test scripts are small, maintainable and easy to understand with swift execution of steps. They are independent of each other and run with good exception handling.                                                               |
| Code review              | Code review or static testing is a systematic check of another’s code for mistakes based on standards and guidelines.                                                                                                                                                                                                                                             |
| Debugging                | The process of finding the cause of a problem in a software code.                                                                                                                                                                                                                                                                                                 |
| Utilities                | Contain the functions required at a generic level; these are not application specific.                                                                                                                                                                                                                                                                            |
| Verifications            | Contain the validation functions that are application specific.                                                                                                                                                                                                                                                                                                   |

12.2 BUILDING A TEST AUTOMATION FRAMEWORK

This section explains how to build a test automation framework. The process and components of a test automation framework can be better understood by going through a real case study of one developed for a public-facing web-based healthcare portal.

This test automation framework was created to last a decade to cater to functional and regression needs. The test automation architect is the key person responsible for developing and maintaining the test automation framework. They define the coding standards and train the test automation engineers to write automated test scripts.

The key steps to developing this framework were:

1. Framework requirements and scope
2. Test automation framework approach
3. Tool selection
4. Phases of the automation
   1. Initial phase
   2. Development phase
   3. Final phase
5. Defining framework folder structure
6. Complying with guidelines and standards
7. Test script and execution

The above steps will be explained below in the context of the healthcare portal.

12.2.1 Framework requirements and scope

The SUT was a web portal for a multimillion user base that helps users to make choices about health, from lifestyle decisions to the practical aspects of finding information when needed.

This section provides an overview of the scope of test automation – what is automated and what is not. The focus was mainly on the overall need for functional and regression testing. The requirement was the test automation framework development, creation of the regression suite and execution of the created automated scripts.

The framework was expected to support the multiple browsers, operating systems, mobile platforms and environments as shown in the below table.

Table 12.2 Framework platform requirements

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/tab12-2.png)

The framework and the test suite were expected to be independent of any environment and build. The following functionalities and features were in scope:

- Content management
- Large set of test data validation
- Backend systems

The following functionalities and features were not in the scope of this framework due to the high level of effort required for minimal returns.

- Videos, audios and embedded flash testing
- User interface and user experience

12.2.2 Test automation framework approach

A test automation framework approach or plan is a document describing the approach to the automated testing and framework. This is the top-level plan generated and used by the test automation team to direct the test effort. This document describes ‘how’ automated testing is implemented for the solution and ‘when’. This provides a summary of the test automation activity and responsibilities specific to the life cycle of the framework. The key steps to forming a test automation framework approach or plan are:

1. Identifying the functional areas or products for automation, for example web services, healthcare.
2. Analysing the functional requirements and test cases, for example review the SUT features and test scenarios for the suitability of test automation.
3. Verifying the feasibility of automation such as the compatibility of the SUT with the selected tool, for example proof of concept to ensure that the proposed tool is compatible with the SUT and is fit for purpose.
4. Identifying the manual tests that can or cannot be automated, for example tests involving frequent manual intervention or UI/UX.
5. Classifying the test cases or requirements into various levels or priorities based on business needs, for example critical features, frequently executed tests.
6. Developing the test automation framework, for example framework libraries.
7. Automating the level one or priority one test cases and requirements for the initial set of tests. The time-consuming manual tests can be expedited and added to this list as well, for example regression tests or build validation tests.

12.2.3 Tool selection

This section addresses the test automation tool selection criteria for the healthcare portal. The test automation tool for the healthcare portal was selected based on the following factors:

- The priority was the test automation tools that were widely and commonly used for functional test automation. This ensured good support from the vendors, community and the availability of skills in the market.
- Latest version of the tool based on a PoC result. This ensured that the tool was compatible with the SUT and with the latest browsers available in the market.
- The SUT was developed on Microsoft .NET and SharePoint, and the selected tool was flexible and suitable for Microsoft .NET and SharePoint platforms.
- The selected tool supported test script execution on multiple environments and platforms and in batch mode in order to save time and effort.

12.2.4 Phases of the automation

The **software test automation framework (STAF)** was based on common library functions, which increased the flexibility of the framework. Automation framework development was carried out in three phases: initial, development and final.

Initial phase

The purpose of the initial phase was to plan the test automation framework with activities such as understanding the solution, analysing the SUT, setting the criteria for candidate selection for tests, defining scripting standards, following guidelines and formulating a test automation framework plan.

The following activities were part of the initial phase:

1. Understanding the architecture and functionality of the SUT.
2. Identifying the application functional areas and tests to be automated.
3. Developing the scripting approach.
4. Agreeing on the automation framework approach and plan.
5. Designing test automation framework, scripting standards and guidelines.

Development phase

The objective of this phase was to create the automation framework based on the plan developed in the initial stage. At the end of this stage a test automation framework and initial set of test scripts were ready for the product.

The following activities were part of the development phase:

1. Defining, creating and collecting test data.
2. Building common libraries of the framework.
3. Creating test automation scripts for prioritised tests.
4. Executing the trial or initial test scripts (dry run).
5. Analysing the test results from the test execution and test reports created by the framework.
6. Peer reviewing the test scripts.
7. Preparing the user manual for framework, script maintenance and execution.
8. Sharing the framework and test scripts with the wider testing, development and support teams.
9. Enhancing the test scripts for additional features and products.

Once the test execution is completed, the next step is to review the test results and identify functionality or components that experience a relatively high number of failures. The result analysis summarises whether it requires additional test effort to update or enhance the tests scripts and framework. Test results and reports generated from the analysis can confirm the executed test scripts are suitable to identify defects in the SUT. It is the last phase of test automation framework development and thereafter the test reports are shared with all stakeholders.

Figure 12.1 Test automation road map

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-1.png)

Final phase

The final stage was to transition the automation framework, scripts and related documents including how to set up the framework, user manual and so on to the ongoing support team.

The following activities were part of the final phase of the healthcare test automation framework:

1. Baselining the framework, automated scripts and documentation.
2. Defining ongoing maintenance.
3. Defining a road map.

The above figure presents the road map for the framework.

12.2.5 Defining framework folder structure

The folder structure shown in the below figure represents test data, common libraries, exceptions and automated scripts of the framework. This structure can be further expanded with more reusable components and libraries subject to the automation needs, for example ‘Reporting’.

Figure 12.2 Framework folder structure

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-2.png)

The folders are explained below:

- Data folder contains the test data, which are maintained in a spreadsheet.
- Default_Data contains files that are saved from the SUT.
- Lib folder contains the reusable functions.
- Object repository (OR) contains data related to the objects’ descriptions of the SUT stored.
- Recovery folder contains generic functions to handle exceptions at runtime; all the recovery scenarios are stored.
- Results folder contains test execution result files for every execution of the scripts stored.
- Scripts folder contains test scripts.

The framework could have many more additional components such as:

- Global variables – Environment file can be located here.
- Reporting – Libraries for reporting purposes can be available here.
- Utilities – Functions required at a generic level, and not application specific will be available here.
- Verifications – Contains the validation functions that are application specific.

For the framework created for the healthcare application, the common functions and variables were maintained in the Lib folder. Test data were maintained using Microsoft Excel files and were stored in the ‘Data’ folder. The test data could have been directly used from the database.

The below figure provides another example of a folder structure for an ecommerce project that used BDD SpecFlow (a .NET open-source framework for behaviour-driven development, SpecFlow helps BDD to turn specifications into executable code).

Figure 12.3 BDD SpecFlow for an ecommerce project (example)

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-3.png)

The folders are explained below:

- Features – Documents that contain Gherkin scripts and other relevant details. Feature files allow the building of test packs for features and activities. This helps in creating a set of regression tests that can be maintained more easily than individual stories.
- Model – The model classes represent domain-specific data and business logic.
- Pages – Page Object model is an object design pattern, where web pages are represented as classes, and the various elements on the page are defined as variables of the class.
- Properties – Programming language properties such as .Net or Java.
- Report – Execution reports are stored in this folder.
- Steps – Step definition is a piece of code with a pattern attached to it or, in other words, a step definition is a Java method in a class with an annotation.
- TestBase – This folder contains the files, browser selection classes, web extensions and so on.

12.2.6 Complying with guidelines and standards

The automation scripts for the healthcare test automation framework were developed based on coding standards, guidelines and naming conventions. A proper naming convention based on the agreed standards and guidelines was followed for variables, functions and objects. Comments were specified in the code wherever necessary for ease of later maintenance. A proper indentation is used for a clear understanding of the script. The indentation refers to the space at the beginning of a code line.

12.2.7 Test script and execution

The test automation framework for the healthcare portal was developed by following a hybrid automation approach. This was a combination of a data-driven and a keyword-driven approach. All the test scenarios were built on the data-driven approach to broaden the scope of testing by using various sets of test data (parameterisation).

The execution was initiated from the ‘application sheet’. This sheet maintains data related to environment, browser and application functionality. The below figure provides an example of the application data sheet from the healthcare test automation framework.

Figure 12.4 Application data sheet

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-4.png)

The application areas or modules were maintained in a separate sheet based on the category. This sheet was used to define the scope of any regression testing. The regression test suite was designed by updating the sheets with relevant values. The application areas or modules could be selected through the data sheet with yes or no values.

The below figure provides an example of the application areas/modules data sheet from the healthcare test automation framework.

Figure 12.5 Application areas/modules data sheet (regression suite)

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-5.png)

It is necessary to update a data sheet and execute the test if a new environment is added the requirement.

The below figure provides an example of the regression test data sheet from the healthcare test automation framework.

Figure 12.6 Data sheet (regression suite)

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-6.png)

After every test execution, a report was generated based on the selected environments, browsers, operating systems and application functionalities. This report was generated in HTML format by the reporting scripts created as part of the framework, stored in the results folder and was scheduled to be sent automatically to various stakeholders by email.

Figure 12.7 provides an example of the test report from the healthcare test automation framework.

Figure 12.8 provides an example of the test execution summary from the healthcare test automation framework.

Figure 12.9 provides an example of the detailed result from the healthcare test automation framework.

This section has provided an overview of the structure and components of a real-life hybrid test automation framework for the healthcare portal. It is to be noted that the creation of a framework was subject to various factors such as tool availability, SUT, skills, ROI and scope of automation.

12.3 SUT ARCHITECTURE

Good knowledge of the SUT and its architecture is important for test automation framework design. The solution architecture design document or full system architecture document is a good place to go to understand the SUT architecture. The physical and logical architecture design documents provide insight into server types, network architecture, storage requirements, interfaces, network design, system components, related components, sub-components, data architecture, security architectures, the generic structure of the solution, logical information, capacity and service continuity. This information can be located from the following placeholder documents of the SUT:

Figure 12.7 Test report

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-7.png)

Figure 12.8 Test execution summary

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-8.png)

Figure 12.9 Detailed result

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-9.png)

- The solution architecture design or full system architecture – Defines the generic structure of the solution, providing the logical and physical information architecture for the selected option, including all related components and interfaces, capacity and service continuity designs.
- Detailed design and physical design – Defines the design of the physical architecture of the selected logical option, server types, network architecture, storage requirements and interfaces. This also includes any network design.
- Security architecture and cybersecurity assessment – Provides insight into the security aspects and risks associated with the implementation of the solution and used subsequently to show that security has been adequately considered. It highlights the threats and vulnerabilities and investigates countermeasures to provide assurance to the business that adequate security has been implemented.
- Component design architecture or low-level design – Provides the detailed architecture for a component. It describes the services a component provides, its sub-components and the supporting architectural views for a component, for example application, data and security architectures.
- IT business and service continuity – Details the instructions required to failover or restore a system or service in the event of failure.
- Test strategy and plan – Defines the strategy for the assurance and testing effort required for the solution. It provides a summary of the test stages and responsibilities specific to the product or project. It may be high level (dependent upon availability of functional and non-functional test requirements) and elaborated in the next phase. This includes all the information necessary to plan and control the test effort for the solution development phase. It describes the approach to the testing of the artefacts and is the top-level plan generated and used by managers to direct the test effort.

It is essential to comprehend SUT architecture for the test automation framework design as any failure to understand application architecture and avoid decoupling components in the automation framework impacts the long-term ROI and the maintenance of the framework. For example, failure to separate the UI of an application from the automated tests will affect all related automated tests due to any minor change to the UI of the SUT.

High-level design and full system architecture are sources of information on how the overall system applications are developed as part of their overarching enterprise architecture, including what technology is used and how these subsystems interact with each other to meet the overall business needs.

12.4 TEST DATA MANAGEMENT

Data management and maintenance is a key part in any organisation. Many automation frameworks facilitate their own data management by gathering data from the business and maintaining them as part of the framework. Test data are the input given to a SUT during test execution and are used to validate both normal and alternative conditions. The positive data (input) are used to verify that functions produce expected results, and the negative data (input) are used to check unusual, exceptional, abnormal or unexpected outcomes.

A process of planning, designing, storing and managing data for a SUT is called software test data management.

One of the key challenges for test automation is managing test data. Test data are key for the application to work well with the automation tool. Lack of accurate and realistic live-like data will be impractical for automation. Test data can be created, or existing test data from different environments can be considered for test automation. However, it is not always possible or feasible to transfer data from one environment to another for technical and data protection reasons.

Test data should be defined and should be available prior to performing automated testing, unlike manual testing data, which can be created during test execution. Defining these data are an integral part of developing both the manual test scripts and automated test scripts.

There are various challenges in defining and creating test data. These challenges should be addressed prior to scripting. The list below describes some key challenges in test data management:

- Data change often – This can cause a particular test to fail and creates a new requirement for additional or new data. The test script can be programmed to accept a level of tolerance to overcome this situation.
- The business does not have the time to verify the data with the automation team – This creates a dependency on the business, which is always a bottleneck when performing automated testing. The automation framework should be programmed to collect the data directly from the source if possible.
- Errors in data imported to the framework – This is a key issue, specifically in transactional test data. The automation framework should be programmed to collect the data directly from the source if possible.
- GDPR and PII data cannot be shared with the test team – Due to the strict GDPR and PII guidelines, it is not often possible to use real-life, personal data for automated testing. The automation framework should be programmed to collect the data directly from the production or a production-like environment if possible. The test automation framework can be installed and configured on the production environment to avoid any data breach. The test execution environment needs to be accredited prior to using PII data.
- Data integrity and data accuracy – This is a key issue when data are created manually or when using a tool for testing. The automation framework should be programmed to collect the data directly from a production-like environment, and the test environment refreshed from the production or production-like environment prior to test execution.
- Environment accreditation – A prerequisite for many secure and financial systems is to use live-like data or data from the production system. The test execution environment needs to be accredited prior to using PII data. The accredited process is generally effort intensive and involves multiple teams.

Test automation starts tackling the data from the planning stage, as waiting until the automated test execution stage is too late and impacts the testing. The solution needs a comprehensive test data strategy in place prior to automated testing. Test automation can also reuse the data from the manual testing or the data created by load and volume testing. Test data can be created in different ways. The list below and the below figure cover different methods and sources of data for test automation. These are subject to your SUT and business domain.

- Manually created data – For example, use the data from the manual testing.
- Test data creation tools – For example, use test data creation tools such as DATPROF, Informatica Test Data Management or InfoSphere Optim.
- Production data – Use the data from the source or the live system for test automation.
- Test automation tool/framework-created test data – Use the test automation framework to create the test data such as user accounts.
- Purchase – Different types of test data can be purchased such as postal, telephone or email, for example from organisations such as UK Datahouse or Data HQ.
- Existing data – The data used for the previous automated testing cycle can be used again for the next cycle.

Figure 12.10 Test data creation

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig12-10.png)

Test data are generally different from production data. However, often production data are used as test data. Test data management tools are widely used to manage data for manual testing and test automation.

The below table covers a set of widely used test data management tools, and their key features.

Table 12.3 Test data management tools

|                                                    |                                                                                                                                                                                                                                                                                                 |
| -------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tools                                              | Key features                                                                                                                                                                                                                                                                                    |
| DATPROF test data management tool                  | A test data management tool for data maskingProvides synthetic test data generation and a test data provisioning platformManages and refreshes test data across environments from one central locationCompliance with GDPRIntegrates and automates various test data processes within the CI/CD |
| Informatica MDM                                    | Provides automated data subsetting, data masking, data connectivity and test data-generation capabilitiesProvides cloud-based solutionManages multiple domains such as customer, product or supplier                                                                                            |
| CA Service Virtualization (formerly known as LISA) | Simulates the behaviour dataCreates a virtual data setImports test data from different types of data sources such as Excel sheets, XML and log filesAutomatic data masking protects sensitive data without violating any security policy                                                        |
| IBM InfoSphere Optim                               | Offers data management from requirements to retirementSupports continuous testing and Agile software developmentProvides real-time data testing                                                                                                                                                 |

12.5 SUMMARY

Test automation makes software testing easier, faster and more reliable if implemented correctly and is essential in today’s fast-moving software delivery environment. Usually seen as an alternative to time-consuming and labour-intensive manual testing, test automation uses software tools and frameworks to run a large number of tests repeatedly to make sure an application does not break whenever new changes are introduced. This chapter summarised how to design a test automation framework and components of the framework. This chapter also addressed the importance of SUT architecture and test data management in test automation.

The next chapter addresses another key area in test automation: how to measure the progress, status and success of test automation and KPIs.
