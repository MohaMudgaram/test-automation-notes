## TEST AUTOMATION AND TEST COVERAGE

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

Test coverage is used as an indicator to measure the quality and effectiveness of software testing. It is a method used to determine coverage of tests of the application code and amount of code that is exercised when the tests are run for example. If there are 100 requirements and 100 tests created for 100 requirements with 90 tests being executed, then the test coverage is 90 per cent. This helps to understand the gap in testing and create additional tests for solution coverage. Test coverage helps quality assurance ensure quality of the test, gaps in test cases, code coverage, testing scope measurement and defect prevention.

Test coverage is widely used for test completeness and test automation is a widely accepted method to increase test coverage quickly. Test coverage and test metrics provide enormous confidence to the stakeholders. Test automation provides 100 per cent test coverage in some areas such as unit testing, performance testing, security testing and data validation. The most commonly used metrics are related to test execution efficiency, automation coverage, effort reduction, additional test cycles achievement, **defect detection trends (DDT)** and so on. This chapter addresses the value of test automation in test coverage.

8.1 TEST COVERAGE

One of the widely accepted ways to measure test coverage is based on functional and non-functional requirements. The functional and non-functional requirements drive what is expected from the application. Functional requirements describe the application’s expected behaviour, and non-functional requirements describe the reliability and sustainability of the application.

Requirement coverage is not always achieved through testing or test automation, as many requirements such as legal, standards and compliance are achieved through static testing and verification. A **test traceability matrix** is the most common method to track the requirements until the final application, and test automation ensures test coverage is met quickly and consistently. Various tools such as Micro Focus ALM, Microsoft Azure DevOps and Jira are available for the **requirement traceability matrix (RTM)**.

‘Traceability is the degree to which a relationship can be established between two or more work products. A traceability matrix is a two-dimensional table, which correlates two entities, for example requirements and test cases. The table allows tracing back and forth the links of one entity to the other, thus enabling the determination of coverage achieved and the assessment of impact of proposed changes’.

Requirement coverage and code coverage are two different concepts, even though they are often used to measure the same result. Code coverage is a common unit testing practice that is widely used to measure how much of the code is actually being used in the unit tests, how much code is not being used in unit tests, and also shows which branches are and are not being covered. Unit testing is part of the software development activity, and the responsibility lies with the programmers or developers. There are various tools available to check and optimise the unit code coverage.

Requirement coverage is the responsibility of the testing team. They validate that the tests have covered all the test conditions that were derived from the requirements and other acceptance criteria. A requirement traceability matrix is often used to trace the requirements until acceptance and is a key parameter in deciding when to stop testing.

This section will address some of the most common test coverage methods widely used in the industry and added value provided through test automation.

8.1.1 Unit test coverage

Unit tests are typically written by programmers to validate the correctness of the code. This is to verify that the code has been programmed in line with the program standards and LLD or **detailed design document (DDD)** derived from the product backlog or the requirement specifications.

LLD or DDD defines the design of the physical architecture of the selected logical option, server types, network architecture, storage requirements, interfaces, network design and so on.

Unit testing is generally expected to be 100 per cent automated by using appropriate tools. However, if the effort versus value benefit does not weigh up, unit tests should not be conducted, for example a simple call to API with no business logic in the code will not be unit tested as it would be a significant effort for very little benefit. Code coverage basically shows how much of the code is being used in the unit tests. Code coverage also demonstrates which branches in conditional logic are not being covered. A line coverage measures how many statements or lines of code are covered. Branch coverage ensures that each one of the possible branches from each decision point is executed at least once.

CIT, also known as unit integration testing, is to verify that the program components are all present and can work together. The CIT should be 100 per cent automated, where possible. Product-based organisations place high emphasis on unit testing. Unit tests are generally either performed manually or automated, with a wide-ranging set of tools available for automation. Some organisations pay less attention to unit testing as it is time-consuming and slows down the solution development progress. Unit testing improves the quality of the software solution and identifies the defect much earlier in the defect cycle. Unit tests are often developed at the LLD and performed at the micro-level. The key inputs for the unit test are the product backlog catalogue or requirements, style guide, code or component units and LLD. They are generally performed on the development environment and development workstations. Off-the-shelf software tools and package vendors generally provide an inbuilt testing framework known as the **automated test framework (ATF)** for unit testing.

The purpose of unit testing is to detect implementation errors in units of code, for example a method or stored procedure.

There are many industry-wide tools and frameworks available for unit testing, for example Java-based and .Net based, to support developers. Many packaged tool providers such as ServiceNow and Oracle provide their own unit test suite to support the unit testing. These test suites, generally known as ATF, are inbuilt in the solution and provided as part of the packaged tool or COTS software.

The key purposes and benefits of unit testing are:

- Good practice, providing quality at a micro-level.
- Finds the defect earlier and at the design level.
- Each basic component or bespoke unit of code functions according to its design specification.
- Exposes issues in the interactions between component units.
- Validates component performance.
- Accessibility compliance for custom code.
- Validates coding standards.
- Checks automated build passed.
- All installation, configuration and data transformation processes are successfully performed.

Automated unit testing reduces manual intervention, and the tests are coded in a programming language with tools and execution against the code base as part of the build process. These automated tests are executed every time after a code build or release, and results are reviewed for errors. Developers use the unit test result to validate the quality of their code.

Automated unit testing provides huge benefits to the test coverage. The key benefits are:

- Used frequently without additional costs compared to manual testing
- Makes the development process more flexible
- Automatically checks the standards, compliance and guidelines
- Makes it quicker to find problems in the development cycle
- Uncovers errors during coding and speeds up development
- Tracks and monitors code quality all the time
- Quicker build validation, easy refactoring and cleaning up existing code
- Quick and detailed test coverage supporting quicker bug fix, hotfix and release

8.1.2 Functional and regression test coverage

Functional testing provides test coverage on functional requirements. The test scenarios and test cases are mapped to requirements to ensure that they have coverage on specifications. Automated test scripts are directly mapped to functional test cases and requirements providing a good indication of test coverage. A well-designed automated framework helps to achieve test coverage quickly and efficiently. An automated requirement traceability matrix provides real-time coverage on requirements and is very useful for large projects and product development.

Test cases are prioritised, and a subset is selected for regression testing. The scope of the regression test pack varies subject to the scope of the release, such as full release, hotfixes, patch release and regular releases. An automated regression pack derived from requirement mapped to the regression pack provides immediate visibility on test coverage. Manual regression testing is monotonous, and less effective once the frequency of the test execution is high, if done incorrectly. Testers tend to ignore the test, and test execution becomes a ‘routine’ rather than a thought-through activity. Test automation is a good method to make it more effective and extensive using different data sets. Test automation is the most suitable test coverage method for regression testing.

In regression testing, the previously executed test cases are re-run, time after time, on a new build, which is time-consuming. The test cases and expected results are available from the previous execution, and automating these test cases is a time-saving and efficient regression test method. Selecting test cases for automation is performed based on various factors such as risk, ROI, the time factor, dependencies and high volume of data.

Smoke testing is generally used to validate whether or not the deployed build is stable and ready for further detailed testing. It is generally performed by the build and deployment team or the test team. Most of the smoke tests are automated, and they are expected to provide quick results. In general, smoke tests are 100 per cent automated and provide full test coverage on build validation.

Automated functional tests provide quick results and full test coverage. Integration testing is an extension of functional and system testing, and the same automation principles are applicable for integration testing. Technical integration tests such as web services testing, API testing and interface testing are generally fully automated and provide 100 per cent test coverage.

The key features of automated functional testing in order to provide test coverage are:

- Provides consistent test coverage
- Automatic coverage of the standards, compliance and guidelines
- Complete test coverage on smoke testing
- Quick and detailed test coverage of functionality

8.1.3 Non-functional testing coverage

Non-functional testing is checking the non-functional aspects of the system, such as performance, usability, reliability, security, accessibility and infrastructure of a software application. It is to test the readiness of a system according to the non-functional requirements. Test automation is a suitable solution for a wide range of non-functional testing, as manual testing is not effective or feasible. Automated non-functional testing is quick and provides full test coverage on requirements. Most of the non-functional testing is fully automated and provides good test coverage, for example performance testing, security testing, browser testing and mobile testing can be fully automated and provide 100 per cent test coverage. However, usability testing, user experience and infrastructure testing are difficult to automate and provide less test coverage.

Key benefits of automated non-functional testing to test coverage are:

- Automated performance, volume and scalability testing provide high test coverage compared to manual testing.
- Tools and automation are essential for consistent test coverage in security testing, for example penetration testing or vulnerability scan.

8.1.4 Challenges in measuring test coverage

Test automation brings speed, confidence, efficiency, reliability and completeness to test coverage and is essential in software testing. However, there are a few challenges in using automation for test coverage.

- When requirements are incomplete, testing is difficult to automate and is unable to provide accurate test coverage.
- The low priority requirements may not qualify for automated testing. This can reduce the level of test coverage through test automation.
- Test coverage in different test stages has a different meaning. Test automation is high for automated unit testing. UAT is generally performed manually and may not be a good candidate for automated test coverage.
- The requirements that are hard to automate are not considered for automation and automated test coverage.
- One hundred per cent automation and test coverage through automated testing are difficult to achieve, for example in usability testing.

8.2 TEST AUTOMATION METRICS

Test automation metrics are vital for test coverage and in ensuring the quality of automated testing. Test automation is a huge investment, and it requires continuous monitoring, tracking and measuring to ensure that it returns the expected benefits and provides ROI. The investment in test automation and automated testing cannot be justified if it cannot be measured.

‘You can’t manage what you can’t measure.’ (often attributed to W. Edwards Deming, the statistician and quality-control expert credited with having launched the Total Quality Management movement, and at other times it is attributed to Peter Drucker).

The investment in test automation and automated testing cannot be justified if it cannot be measured.

- Percentage of test automation coverage
- Percentage of tests passed versus failed
- Percentage of automated tests passed versus failed versus manual tests passed versus failed
- Number of defects found by automated scripts over time to assess the effectiveness of the script
- Number of defects found in manual testing versus automation
- Requirements coverage by automation
- Test automation effort versus manual testing effort

8.3 SUMMARY

In this chapter, we addressed how test automation enhances test coverage. The investment in test automation cannot be justified if you are unable to measure it. Test automation metrics provide a reliable method to measure the return on any investment, understand which parts of the testing are working, and support improvement.
