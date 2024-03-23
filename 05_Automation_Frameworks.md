## AUTOMATION FRAMEWORKS

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

This chapter is essential for all senior test automation professionals – such as managers, leaders, project managers and other decision makers of the automation framework. It details the test automation framework, widely used frameworks, and the advantages and disadvantages of each. This chapter also addresses how the frameworks manage data and the philosophy of using function libraries of automated test frameworks.

A test automation framework is a set of rules followed in a systematic way to deliver targeted results. It is a platform developed by integrating various hardware and software components, along with using various tools for test automation. It is an integrated solution of function libraries, test data, object details and various reusable modules.

A test automation framework is a programming framework that consists of a comprehensive set of guidelines to produce beneficial results from the automated testing activity.

In general, a test automation framework is created through the use of programming languages such as Python, Pearl, Java, .NET and Shell script or testing tools such as Selenium, UFT, Tosca and Eggplant to fulfil a specific need.

The framework should be fit for purpose, support the current and future products and applications in the infrastructure estate, and independent of programming languages, if possible, to support the team in building knowledge and expertise quickly.

The benefits of the test automation framework are:

- Efficient automated test script development
- Provides a structured development methodology to ensure the uniformity of design across multiple test scripts to reduce dependency on individual test cases
- Reuse of components and code
- Reduces dependence on teams by automatically selecting the test to execute according to test scenarios
- Improves the utilisation of various resources
- Ensures an uninterrupted automated testing

The key features of any framework are:

- Runs more tests per cycle.
- Minimal manual intervention.
- Returns quicker results.
- Reusability of codes and components.
- Enhances efficiency of script development.
- Provides a structured development methodology.
- Reduces dependency on individual tests.
- Ensures uninterrupted automated testing.
- Low cost maintainability.
- Improved failure recovery and exception handling.
- Automated test execution dashboard and reports.
- Optimal error handling process.
- Test data remain independent of the code.

The most widely known test automation frameworks are:

- Linear testing framework
- Modular testing framework
- Library architecture testing framework
- Data-driven testing framework
- Keyword-driven testing framework
- Hybrid testing framework
- TDD testing framework
- Behaviour-driven development (BDD) testing framework

This chapter describes the various test automation frameworks in detail.

5.1 LINEAR TEST AUTOMATION FRAMEWORK

The linear test automation framework is generally known as the record-and-playback framework, and it works in linear or sequential mode. Tests and test scripts are created individually and executed one after the other.

Figure 5.1 Test automation frameworks

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-1.png)

In linear scripting, the test actions mimic the actual user actions that would be performed while using the application. The scripts can be written from scratch and they are usually implemented by a tool that provides a ‘capture and replay’ facility. This operates by capturing the user actions and system responses and recording them in an appropriate scripted format. The scripts can then be re-run as required.

A leading global active asset manager and investment firm revamped a core asset-management discipline. Testing was a key activity in the SDLC, and test automation was a key solution for continuous releases. The test team found it difficult to automate the functionality due to a lack of domain knowledge. The business analysts and product owners used record and playback to create the initial automation suite. This was a starting point for the test automation team, and the team enhanced the scripts and converted them to a competent linear automation framework for the SUT.

Advantages:

- Simple and does not require advanced technical knowledge.
- Does not require writing code.
- Generates test scripts quickly.
- Well-suited to create a proof of concept.
- Automation can be introduced very quickly.
- No programming skills are required since it is click and record.
- Linear framework requires no technical or programming knowledge.
- Quick to create a linear framework.
- Low learning curve.
- No initial development or learning effort.

Figure 5.2 Linear test automation framework

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-2.png)

Disadvantages:

- Not reusable and requires high maintenance.
- Test data are hard-coded and difficult to maintain.
- Limited coverage on test data.
- Lacks integration between test cases.
- Difficult to run a large set of test cases.
- No effective error and exception handling.
- High manual intervention.
- The script is only applicable to the recorded set of actions.
- Changes to the SUT results in the updating of numerous recorded scripts.
- Change in application workflow requires high rework.
- Lack of scalability.
- The scripts capture all the user actions, including any incorrect ones.
- The script may become inefficient due to repetitive user actions (e.g. repeated browser back button usage).

5.2 MODULAR TESTING FRAMEWORK

The key feature of the modular testing framework is to divide the system under test into stand-alone and logical ‘modules’ based on the OOP concept known as ‘abstraction’. Independent test cases are developed for these modules and together build a larger test suite for the solution. These modules are separated by an abstraction layer, and changes made to one part of the solution or the framework has a limited impact on the overall framework.

The modular testing framework follows these steps:

1. Analyse the SUT
2. Identify the reusable workflows and develop manual test scripts
3. Create common and separate functions and units
4. Develop automated scripts for the workflows
5. Create a master script to invoke the individual and functional test scripts
6. Combine tests sequentially to create a test suite for the modular framework

The key approach for the modular testing framework is the use of the abstraction layer, and this helps to avoid changing the overall framework whenever there are changes to individual sections. The corresponding module and the associated individual test script need to be changed if there are changes made to the application.

Figure 5.3 Modular test automation framework

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-3.png)

Advantages:

- Low maintenance
- Well-structured modules
- Ease of use
- Less effort to create test scripts
- Reusability
- Easy reporting and debugging
- Scalability
- High team productivity, efficiency and accuracy
- Quick ROI

Disadvantages:

- Data are hard-coded and embedded.
- Difficult to use different data sets.
- Basic framework and is time-consuming to maintain the framework.
- High maintenance required.
- Programming skills are required to develop the framework.

5.3 LIBRARY ARCHITECTURE TESTING FRAMEWORK

The library architecture testing framework is an extended and enhanced version of the modular testing framework. The framework is built based on the library approach, which involves setting up common functions under a library and accessing those functions in the test scripts. This is a more structured and maintainable framework compared to the modular and linear frameworks. Library architecture is more intelligent and organised compared to a generic modular framework.

Advantages:

- Developed on modular framework architecture
- Overall low maintenance
- Scalability
- Cost-effectiveness
- Reusability

Disadvantages:

- Abstraction maintenance is difficult.
- Good technical knowledge required.
- Test data maintenance is complex.
- Highly technical.
- Test script development is time-consuming.

Figure 5.4 Library architecture test automation framework

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-4.png)

5.4 DATA-DRIVEN TESTING FRAMEWORK

The data-driven framework is a testing framework in which input values are read from data files and stored into variables in test scripts. The data-driven framework and methodology are used to automate and validate applications that require large volumes of test data and swift testing. This framework helps to create test data, calculations, test iterations and permutations with minimal effort. This helps testers validate the solution with different data sets, including positive and negative tests, into a single file and test script.

The driver scripts contain navigation through the program, reading the files and logging the test status information.

The most notable feature of the data-driven framework is its ability to separate test data from code. This allows data to be stored on an external data source to enhance data integrity and security. This helps to use different data in the different testing cycles and supports millions of different data combinations. The main difference and advantage of the data-driven framework over the linear or modular testing frameworks is that the test data are not hard-coded. The data-driven test framework can store and pass the input data from an external data source, such as spreadsheets, text files, comma separated value (CSV) files and databases. Test scenarios can be extended to numerous test cases with minimal effort. Test data can be sourced from a predefined spreadsheet, and a business analyst or SME with no knowledge of the framework can prepare the test data for the automated testing.

Figure 5.5 Data-driven test automation framework

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-5.png)

The framework has the capability to access real-time data from production or live source and validate the solution with the most up-to-date and transactional data without losing data integrity and security. This is ideal for industries such as retail, banking and healthcare where the application requires large data sets for validation.

A large global financial application used the data-driven framework to providing 100 per cent test coverage to validate millions of user accounts. Data validation testing was a key priority for the testing, and data involved **General Data Protection Regulation (GDPR)** and **personal identifiable information (PII)**. Manual testing was not feasible as the data set consisted of millions of interrelated data. There were other challenges to the testing as the test environment was not accredited to store or process live-like PII data.

A data-driven framework was effectively used in this financial application to validate the testing of millions of customers’ data against the production database as part of legal compliance. The data-driven framework was designed and installed on the live environment in such a way that it could access the production database securely and validate data with ‘read only’ permission. This helped the application test all the data against the latest database without any security breaches.

Advantages:

- Test multiple scenarios with fewer lines of codes
- Quick testing of multiple data sets
- Secure test data management
- No test data hard-coding
- Easy test scripts maintenance
- High reusability
- Test script independent of test data

Disadvantages:

- High expertise in programming skills required.
- Framework setup requires significant time and effort.
- Requires continuous data maintenance.

5.5 KEYWORD-DRIVEN TESTING FRAMEWORK

The keyword-driven framework uses a technique to separate keywords or actions and data from the test scripts. The keywords are stored in an ‘object repository’ to allow for better code reusability and less script maintenance. The function of the SUT is stored in a file, usually in a table format with instructions. A keyword-driven framework is a table-driven or action-based testing method. The keywords represent various actions being performed to the application.

The fundamental approach of the keyword-driven framework is to separate the tests into smaller components such as test steps, object and actions. Data are managed separately, and expert knowledge is required to develop the framework. This framework and keywords are also used to run the tests manually.

Figure 5.6 Keyword-driven test automation framework

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-6.png)

5.5.1 Keyword table

The keyword-driven framework is used to speed up automated testing by utilising the keywords for a common set of actions. The framework separates the coding from the test case, test step and data in a table, and this helps a non-technical person to update the keyword, create the data and run the existing framework.

The keywords are stored systematically with an associated object and actions in the object repository.

- Test step description – The action to be performed
- Test object – The name of the web page Document Object Model (DOM) or element, such as Username and Password
- Test data – Such as username and password
- Action – The name of the action such as ‘click’ or ‘select’

The test automation engineers refer to the below table and create test scripts. Test scripts use the keyword from the table for the corresponding actions. During the test execution, the test data are used from the data source for the respective username and password field, executing the relevant script. This avoids using hard-coded test data, specifically sensitive passwords in the script.

Table 5.1 Example keyword table

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/tab5-1.png)

Advantages:

- Minimal scripting knowledge is required to automate new features.
- Keywords are reusable for new tests.
- Low maintenance in the long run.
- Concise test cases.
- Early creation of the framework without SUT.
- Independent of test scripts, keywords and test data.
- Easy comprehension by a non-technical audience.

Disadvantages:

- High technical and programming skills required.
- High development cost.
- Complex and requires detailed design and approach.
- Keywords, object repositories or libraries have to be created up front.
- Continuous maintenance.

5.6 HYBRID TESTING FRAMEWORK

The hybrid testing framework is a combination of one or more frameworks. Previously, the hybrid test automation framework widely used the concepts of keyword- and data-driven frameworks. However, the modern-day hybrid frameworks use the best concepts from various frameworks to maximise the benefits.

Figure 5.7 Hybrid test automation framework

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-7.png)

The key to developing a hybrid testing automation framework is choosing the right tool for it. It is important that the framework adapts to the SUT and the other variables involved in its delivery. Most frameworks turn out to be hybrid over a period. Hybrid frameworks that use the concepts of keyword-driven and data-driven approaches tend to be more successful in test automation.

Advantages:

- Fit for various applications.
- High adaptability.
- Granularity of test reporting.
- Extensibility.
- Best concepts from various frameworks.
- Accurate and highly efficient.
- Test data, functions, tests and libraries, for example, are separated.
- Reusability of code.
- Good for testing large data sets and complex applications.
- High ROI over a period.
- Good test coverage.
- Improved failure recovery and exception handling.
- Minimal manual intervention.
- Detailed dashboard.

Disadvantages:

- High and continuous maintenance.
- Considerable technical knowledge and expertise in the scripting language is required.
- Time-consuming.
- Requires detailed test plan and architecture.
- High learning curve.

5.7 TEST-DRIVEN DEVELOPMENT TESTING FRAMEWORK

TDD is generally considered a development technique and unit testing approach. However, TDD is widely used for DevOps. Hence, it is generally used along with the automation frameworks mentioned in the previous sections.

The main concept of TDD is to write unit tests first before you develop the code. The test fails the first time round as there is no corresponding functionality that is developed. TDD develops better software and is primarily driven by predefined tests, thereby increasing the speed of tests and accuracy.

Advantages:

- Defines acceptance criteria up front.
- Reduces the risk of interpreting the expected behaviour.

Figure 5.8 Test-driven development

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-8.png)

- Focused and productive development team.
- Higher code quality.
- Follows good coding practices and guidelines.
- Creates an automated regression test suite.
- Speeds up the development productivity in the long term.
- Clarifies dependencies much earlier in the development cycle.
- Reduces code and requirements-related defects.
- TDD levels up the quality.
- Tests are usually written for different scenarios.
- High ROI.
- Detailed and documented unit testing.
- Follows the approach ‘test first and develop the SUT later’.
- TDD results in more tests.
- Better code coverage.
- Reduces the percentage of bugs.
- The quality of the product developed with TDD is significantly higher.
- Documentation can be used further on for any purposes.

Disadvantages:

- Errors in TDD tests cases will increase defects.
- High up-front time and effort.
- Initially slows down the development.
- High effort to maintain the test suite.
- Continuous housekeeping.
- Unit tests are hard to write up front.
- Hard to develop across all environments, such as legacy systems.
- Highly misunderstood and referred to as ‘functional testing’.
- Takes time to make these tests.
- Developers can focus on the test more than the actual functionality and code itself.
- Lacks code optimisation.
- Increases the development effort.

5.8 BEHAVIOUR-DRIVEN DEVELOPMENT TESTING FRAMEWORK

BDD is considered an extension of TDD as the process is designed to enhance the delivery of software development projects by improving the communication between engineers and business professionals. BDD ensures all projects remain focused on delivering what the business needs while meeting all the requirements of the end-user.

BDD is suitable where the business owner is familiar with the unit test framework. In BDD, test cases are written in a common language used by the business. BDD enhances collaboration between the technical and business teams.

BDD scenarios focus on the expected behaviours of the target application. This helps the project team to work collaboratively and ensures they are on the same page. The BDD scenarios are used as requirements, acceptance criteria, tests and candidates for test automation. BDD frameworks enhance test automation as it directs the test automation engineer to develop a method or function for the corresponding actions.

Cucumber is a widely known test automation framework for BDD, and in Cucumber the BDD specifications are written in plain English using Gherkin language.

Figure 5.9 Behaviour-driven development

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig5-9.png)

Advantages:

- Strong interactions between the project team and the business.
- BDD increases and improves collaboration.
- Software design follows the business value.
- Solution development meets the user needs by focusing on the business needs.
- Early discovery of the unknowns.

Disadvantages:

- Time-consuming
- More effort in writing automation code for keeping that code in sync with the steps defined in the BDD scenarios
- Difficult to write automated tests up front

Behaviour-driven development is generally used alongside the **acceptance test-driven development**. ATDD is developed based on the end-users’ views. BDD focuses on the application behaviour, and **ATDD emphasises the business requirements**. In TDD, BDD and ATDD tests are written before the implementation takes place. TDD is a development practice, while BDD is a team methodology and ATDD is a user acceptance methodology.

5.9 SUMMARY

In this important chapter, we addressed what a test automation framework is and walked through the widely and commonly used types of test automation frameworks, including the advantages and disadvantages of each. In the next chapter, we will cover another important aspect of test automation, the test environment.
