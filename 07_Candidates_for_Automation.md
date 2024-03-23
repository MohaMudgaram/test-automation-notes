## CANDIDATES FOR AUTOMATION

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

Tests and test cases are the first candidates for test automation; however, they are not alone. Tasks such as test data creation, requirement traceability and test reporting are also great candidates for automation. This chapter describes various steps in choosing the right items for test automation and what you should avoid. Some test cases are suitable for manual testing, and some are unsuitable for automated testing as they do not provide enough benefits. This chapter helps test managers and Scrum masters to understand the factors to consider when choosing suitable candidates for test automation.

Over the implementation period, the team identify more candidates for test automation. The scope of automated testing grows from functional and regression testing to additional areas such as requirement traceability matrix, test data creation or non-functional testing. The below figures show how test automation grows over a period, and additional suitable candidates add to automated testing.

Figure 7.1 Test automation: initial days

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig7-1.png)

7.1 WHAT SHOULD BE AUTOMATED?

In the previous chapters, we have addressed the benefits of test automation, using CBA, ROI and so on. It is essential to know how to choose the suitable candidates for automation. The scope and benefits of test automation are beyond functional and regression testing. More areas can be considered for test automation and automated testing, such as smoke testing, build validation and test data creation. Here are some candidates that can be considered for test automation:

Figure 7.2 Test automation growth

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig7-2.png)

- Business features or user flows that cause considerable damage to the business if they fail; automated testing helps to validate these features frequently.
- Tests that need to run against every build or release of the application, such as smoke tests, sanity tests and regression tests.
- Tests that need to run against multiple configurations, such as different platform and browser combinations.
- Tests that involve large sets of test data or inputting large volumes of data, for example filling in very long forms, as test automation helps to achieve extended coverage, reduction of effort and better reliability.
- Reporting requirements, as automated test reporting reduces manual intervention and generates frequent and up-to-date reports.
- Functionalities and test cases that provide immediate benefits, for example smoke and regression tests in DevOps to examine if the deployed build is stable.
- Tests that require overnight dedication, such as batch processes and reports.
- Repetitive actions such as creating test data for every iteration.
- Repetitive tests such as common tests or prerequisites for multiple tests.
- Tests executed with different groups of data, multiple browsers, environments, complex business logic, calculations, different sets of users, special data, on compliance-related matters such as World Wide Web Consortium (W3C) standards, and security testing.
- High-risk test cases and test cases based on high human error hazard potential.
- Extensive tests with a large set of test data and various permutations and combinations.
- Non-functional testing, such as performance testing, load testing, soak testing and stress testing.
- Tests that are time-consuming and hard to do manually.
- Traceability matrix of large sets of requirements as updating the traceability matrix after every test run is cumbersome.

7.2 WHAT SHOULD NOT BE AUTOMATED?

Test automation generally provides high returns and benefits. However, not all tests and SUTs are suitable candidates for test automation. The following factors should be considered when deciding what is not suitable for automation:

- Test cases that can be done only manually or which should be done manually, for example user experience and usability tests.
- Low value and low priority tests as they do not provide sufficient returns.
- Tests that run only once; the exception is data-driven tests with large sets of inputs.
- Tests involving high additional licensing costs such as special reports.
- Tests that require frequent user intervention.
- Tests requiring ad hoc or random testing based on the domain knowledge or expertise, such as exploratory testing.
- Frequently changing features and outcomes, as they are difficult to automate and validate the expected result against the actual result.
- Tests without predictable results such as scientific simulation.
- Test results requiring instant visual or manual confirmation, for example colours.
- Tests that need a high level of effort to automate and low return such as user interface testing.

The below table is a sample template to identify the suitable candidates for test automation. This template also helps to eliminate items that are unsuitable for automation. Test leaders and automation test managers need to customise this template with the right parameters, subject to their products and solutions.

7.3 SUMMARY

Choosing the right candidates for automation is critical for the success of test automation. This chapter provided factors you should consider when choosing and eliminating candidates for automation. The chapter also provided a template to perform the selection of suitable candidates systematically.

In the next chapter, we will explore achieving test coverage through test automation.

Table 7.1 Candidates for automated testing

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/tab7-1.png)
