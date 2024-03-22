## TEST AUTOMATION: A STRATEGIC VIEW

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

Software testing is the process used to validate that the software solution or product meets requirements and expectations. Software testing also aims to find defects and demonstrate that the software is fit for purpose. There are numerous testing methodologies, types and techniques available to validate the functional and non-functional requirements.

**Test automation is the process of using other software for automating manual testing or manual user actions performed in the application**. Test automation helps to automate testing tasks to be performed with the help of tools known as test automation tools. It is a good idea to validate the software with the help of other software where manual testing is either not possible or time-consuming.

**Automated testing is validating a software solution using a specialised software tool, and typically involves automating functions as part of the testing process**.

1.1 INTRODUCTION

Automated testing is the use of special software, separate from the software being tested, to control and execute tests, including the comparison and reporting of actual outcomes to the predicted outcome. The application is known as the **application under test (AUT) or system under test (SUT)**, and the software used for testing is known as the **automated testing tool (ATT)**.

Testing is necessary for all IT systems, and there are numerous instances of IT systems that have gone live without appropriate testing and ended up with defects, causing financial and reputational damage. Testing is a core activity in any IT solution development and is independent of the software development life cycle (SDLC) approaches such as DevOps, Lean, Agile or Waterfall.

IT projects and testing are carried out under three constraints: **cost**, **time** and **scope**. These three factors, commonly called **‘the triple constraints’**, are represented as a triangle (see below figure). Any changes to the triple constraints create an associated impact on quality, which is measured through testing.

Testing strategies endeavour to create the optimal quality in the solution.

Figure 1.1 Triple constraints

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-1.png)

- Scope. Scope reduction saves testing time; however, it implies that only a core set of product features are tested.
- Time. More time is required for more testing, and this will help to achieve confidence in quality but at an increased cost.
- Cost. Cost is directly proportional to time and scope.

This triple constraint is regularly visited from day one of any IT project due to delay of upstream dependencies, and test managers are often under pressure to shorten ‘time’. **Risk-based testing (RBT)** is one of the widely used approaches to optimise testing time and effort, test automation is another. Risk-based testing and test automation can be combined.

**Risk-based testing is a good solution for managing quality risks due to the reduced time it takes**. Test effort allocation based on the risk of failure is one of the efficient and effective ways to optimise testing. One of the key benefits of the risk-based test approach is **ensuring that the maximum value is derived from the planned testing activities, even when the time available to complete test execution is reduced, by the late delivery of the solution, environment or resource availability problems and so on**.

Risk-based testing is not about risk and issue management per se – it is about managing quality risks – but builds upon these processes to help identify critical areas that require testing focus. All testing activities need to be prioritised to ensure that the most important tests are completed early so that if time available for testing is reduced, the most critical tests can be completed.

A few methods to manage the triple constraints with minimal impact on quality and testing are listed here:

- Start testing or test preparation early, for example informal testing prior to the planned and scheduled testing.
- Involve the testing team from the beginning as part of the business case development or the design phase.
- Reduce duplicate testing such as common tests in system testing (ST) and user acceptance testing (UAT).
- Join up or merge testing cycles, for example the last cycle of system integration testing (SIT) and the first cycle of UAT.
- Introduce the quality assurance (QA) process as a proactive measure.
- Use testing techniques like exploratory testing to find defects.
- Introduce test automation.

**Test automation is a software development project that includes most of the phases in the software development life cycle**. Test automation is widely enhanced by test automation frameworks.

**A test automation framework is a programming framework that includes a comprehensive set of guidelines to produce beneficial results from the test automation activity**. An automation framework is either provided by the ATT or, in some cases, a customised tool, which manages test automation in order to produce a better outcome. A test automation framework generally provides a structure to automation tools that fit its purpose. Most test automation tools provide a default framework for automating the SUT; however, the automation tools can be customised for specific requirements, for example an automation framework that schedules various testing tasks as best fit a specific need, generating custom test reports. Test automation frameworks will be explained in detail through the later chapters of this book.

There are numerous ways to make software testing efficient, and test automation tops the list.

Test automation is a key approach in reducing testing effort, but it is not the panacea to all testing activities. Test automation can be introduced at different stages and phases of the test cycle, such as:

- Product development or solution implementation
- Test management
- Functional and regression testing
- Support (post-live) or run
- Test generation
- Test data generation
- Inspection and evaluation of test results
- Compliance

Test automation is widely used across various industries and applications, and it produces great results. Software development approaches such as DevOps, Agile, Waterfall and their different flavours widely use test automation to reduce cost, increase efficiency and accuracy, and speed up regression testing. Test automation is widely used to reduce cost in the long run. The below figure demonstrates the cost reduction by using test automation over time.

Figure 1.2 Manual testing versus test automation

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-2.png)

Test automation is a strategic decision that is taken based on sufficient data and analysis. However, many projects and organisations approach test automation as simply a method for cost reduction and end up failing miserably. It is not a short-cut to reduce cost, save time and improve the quality of software testing, and should not be treated as such. Various factors such as SUT, technology and life cycle play a major role before considering automation as part of testing. If used correctly, **Test automation is one of the most reliable methods of delivering software testing successfully and securely**. There are numerous challenges in the implementation of successful automation, such as tool identification, skill requirements and ways of working.

1.2 MANUAL TESTING AND AUTOMATED TESTING

This section covers how software testing is generally performed. Software testing is performed in two different ways:

- Manual testing
- Automated testing

1.2.1 Manual testing

**Manual testing is the process of validating a software solution manually**. This often involves a person who mimics the role of an end-user under both normal and unusual conditions. Manual testing also **involves technical checks or exploratory testing**. Manual testing **involves activities such as requirement analysis, risk assessment, identification of scenarios, test case development, test execution, verifying the actual result against the expected result, reporting defects for deviations, updating the test result, and validating the features after defect fixes**. The above tasks are performed by a human in manual testing. Test automation tools can be used to enhance manual testing, such as using a defect management tool to report and track the defects. The section below covers some advantages and disadvantages of manual testing.

Advantages:

- **Suitable for exploratory testing** as this involves creativity and domain knowledge.
- **Effective for short-term projects** as the testing can be quicker than automated testing, avoiding the time and effort needed to set up a tool and perform the testing.
- **Best for single-release projects** as there is no need to create, maintain and perform a regression suite for post-live release. Test automation is unlikely to provide sufficient return on investment (ROI) for a single execution. ROI is covered later in this chapter.
- Humans can notice defects that automation overlooks, for example user interface (UI) testing.
- **Good for user experience (UX) and usability testing**, human intervention is required for these.
- Test execution can start at any time as there is no dependency on tools and infrastructure.

Disadvantages:

- Manual testing is **generally time-consuming compared to the time that the same task will take if done in an automated fashion**, for example data validation testing of large volumes.
- Some manual testing is **tedious to perform**: testing a credit card application for many users by filling out the same form time after time, for example.
- **Heavy investment in human resources** as hiring and training testers requires high levels of effort and investment. Human errors can be avoided using Test automation.
- **Debugging complex defects can be difficult** and might need multiple runs to collect more information.
- Manual test results are not always accurate due to the higher probability of errors compared to machines.

1.2.2 Automated testing

Automated testing is validating a software solution using a specialised software tool, and this typically involves automating functions as part of the testing process. The most common candidates for Test automation are:

- Test management and defect management
- Unit and unit integration testing
- Functional testing
- Regression testing
- Non-functional testing such as performance and scalability

Advantages:

- **Quick and reliable** – Test automation makes test execution quick and reliable. It eliminates human error that can arise in manual testing.
- **Consistent and comprehensive** – The testing will be consistent for any and every data input. The test data set can be increased to 100 per cent coverage. For example in payroll parallel run (PPR), a test automation tool can provide 100 per cent data coverage for all employees in the organisation. Automation tools deliver precise results as testing is accurate, consistent, comprehensive and quick.
- **Repeatable** – Test automation enables reusability by executing the same tests multiple times with minimal cost. This is useful in extending the test coverage to multiple platforms, environments, operating systems, browsers, and mobile devices. Test automation helps to extend regression testing of different platforms, for example multi-browser, and increases test coverage from development to production. Automated testing can repeat the same tests on different data, platforms and environments with limited resources and fewer overheads.
- **Programmable and reusable** – This reduces the dependency on manual interactions and helps with automatic scheduling.
- **Reduces time for testing** – Multiple tests can be executed concurrently, which helps complete testing quickly and reduces the testing timeframe. It also reduces the long-term cost and supports frequent releases of the application by reducing the elapsed time for testing and getting the application to live faster.
- **Improves the productivity of human testing** – Test automation reduces the manual testing effort. It can achieve 24/7 test execution, more importantly, it can be integrated to run automatically when code is committed. Test automation helps ensure a better use of resources, consistency and repeatability of tests.
- **Provides a detailed test log** – The test log and execution report are important in testing. Test automation tools can send a detailed report including pass and fail scores with reasons for failure to stakeholders in different locations and time zones.
- **Highly recommended for graphical user interface (GUI) and performance testing** – Performance testing of large volumes is nearly impossible without test automation. GUI testing on multiple platforms is time-consuming without test automation. Test automation is highly used for non-GUI, API, service level and API testing and is an integral part of ‘pyramid’ and ‘ice cream cone’ models of testing.
- **Assured test coverage** – The test coverage and accurate measurement of quality is guaranteed in automated testing, which is subject to the quality of the automated test suite used for testing.
- Test automation supports all testing types and phases of testing, including functional testing, non-functional testing and test management – Test automation provides significant payback in the future for tests that are difficult to perform manually and require more time.

Disadvantages:

- **Less coverage on negative and exploratory testing** – Exploratory testing is an approach to software testing that is often described as simultaneous learning, test design, and execution. This is less formal and not based on structured test cases and steps. Exploratory testing is very effective when performed by a functional subject matter expert (SME) with an awareness of formal testing. Testing tools have limitations in performing exploratory testing.
- **Static testing and reviews** – Static testing and code reviews are generally performed without executing the code. Testing tools are often limited in performing detailed static testing. However, there are many white-box tools that are effectively used for automated static reviews, for example SonarQube is an open-source platform that is used for continuous inspection of code quality to perform automatic reviews with static analysis of code.
- **Tools incur high costs** – Automation tools incur several costs including infrastructure, maintenance, development and human resources, even if the automation tool is open source or freeware. Automation suites require continuous maintenance. Tools upgrades or patches also often incur high costs.
- **Analysis of the test result is time and cost intensive** – Test automation suites can be developed to validate the result manually; however, any failures require detailed analysis to locate the root cause and are time-consuming.
- **Requires sound coding skills**.
- High maintenance cost – Many functional automation tools are GUI dependent, and maintenance is high if there are any changes to the GUI.
- Not an effective method for short-term products and projects – Automation is generally not suitable for short-term software product development and ROI will be low.
- **The application needs to be stable enough to execute automated scripts** – A stable application is generally required for most automated testing. Functional automation preparation and execution are largely subject to a stable application.
- Software testing tools often introduce their own defects – The defect can be part of the test automation suite and not a defect in the SUT.

1.3 THE ‘WHATS’ AND THE ‘WHYS’ OF TEST AUTOMATION

Test automation is one of the most misused approaches in software engineering. It is very often used as a solution for reducing time and replacement of manual testing. The strengths and weaknesses of Test automation are not often well analysed in many projects. Test automation is neither a solution for all testing problems nor a replacement for skilled manual testers. It is not a solution for reducing testing; instead, it is a long-term investment that pays dividends over a period. Test automation is a software development project that undergoes most of the phases in a software development life cycle. The final solution or product requires continuous maintenance and support. Test automation employs the same software engineering practices that would apply to any software project, and it requires expertise and skills in testing tools and programming languages.

Test automation saves a lot of effort and energy needed for the rigorous testing of the system. It ensures wide and consistent test coverage in the test execution. It helps in achieving 100 per cent validation of large data sets to ensure that no stones are left unturned to provide stakeholder confidence. Test automation can be used to reduce the level of manual testing and manual testers in the long run. Although test automation brings a lot of benefits, the need for manual testing never goes away, but effort could be more focused on exploratory testing, one-off testing (one-time testing) and usability testing.

An example from one of the largest global healthcare portals, with over 500,000 pages and 10 million unique visits a month.

This SUT required the detailed testing of periodic releases, monthly regression testing and data validation testing. The test team consisted of 10 test analysts across functional testing, non-functional testing and test automation. The testing team grew quickly from 2 to 10 members to meet the testing requirements. The application required 100 per cent data validation due to the sensitivity of the information, including data related to public services. The main challenge was the increasing cost and time required to complete the manual regression testing (which took up to 5 days).

A hybrid automation framework was introduced based on a cost-benefit analysis and return on investment. The automation framework helped to ensure 100 per cent data validation and functionality testing on multiple platforms overnight. The good exception handling and reporting modules helped to manage the test execution efficiently and deliver the test execution reports to the stakeholders quickly. A two-member test automation team helped to meet the break-even point within six months and 100 per cent test coverage.

1.3.1 Why test automation?

Test automation provides the following benefits to an organisation and its customers and stakeholders:

- **Increased test coverage and better testing quality** – Test automation can extend test coverage by performing testing of a large volume of data. Test automation can also provide consistency and accuracy in test execution by eliminating human error.
- **Improved efficiency and effectiveness** – Test automation can repeat the same test or the same test with different inputs with less cost and effort, bringing increased efficiency in overall testing.
- **Better reliability and accuracy** – Test automation is more reliable than manual testing as it reduces human error from test execution.
- **Cost-saving and time reduction** – For example, automated regression testing helps to run the regression tests quickly, more often, within different environments, unattended and with large data sets. This will reduce the cost and save testing effort.
- Test automation enhances testing as it can run unattended, reducing dependency on time, place and resources.

The below figure shows the benefits of test automation and why it is required.

Figure 1.3 Why test automation?

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-3.png)

1.3.2 Testing types and test automation tools

Testing can be divided predominantly into two types: **functional testing** and **non-functional testing**. There are a large set of open-source, custom-developed and vendor-provided tools available to support functional and non-functional testing. There is also a third category of testing tools for test management activities such as test planning, test design, defect management, and reporting.

- Functional test automation. Functional test automation tools automate the tests concerning application functionality or how applications function.
- Non-functional test automation. Non-functional test automation tools enhance non-functional requirement testing, that is, the performance, usability, accessibility, reliability, security and infrastructure and so on of a software solution. Most of these non-functional requirements are difficult to test manually. For example, testing a website for thousands of concurrent users is not possible without an appropriate testing tool.
- Test management. Test management is everything the test team does to manage the software testing process, such as test planning, test preparation, test case development, test data preparation, test execution, test matrix, test reports and defect management. Test management tools help test teams to manage the testing process, test life cycle and reporting.

Now we’ll explore another key factor for the success of test automation, stakeholder management.

1.4 MANAGING STAKEHOLDERS IN TEST AUTOMATION

The success of test automation is highly dependent on support from the stakeholders, as automation requires a continuous and long-term commitment to funding, resourcing and sponsorship. Stakeholders vary in different organisations and engagements. In most product-based companies, the immediate stakeholders for automation are internal such as a product owner, product lead, development lead or product manager. There are also generally external stakeholders such as customers, vendors and system integrators.

A stakeholder is any individual, group or organisation that can affect, be affected by or perceive itself to be affected by a programme, product or SUT.

Although testing is a standard phase in the software development life cycle, it is managed differently in product versus **multi-supplier (MS)**, **multi-vendor (MV)**, **system integrator (SI)** and **IT consulting** companies. In product development organisations, test automation budgets are allocated as part of product planning. Here testing tools are mostly procured or established prior to the product or solution development and they are already in place for many matured product development organisations as a part of the **Test Centre of Excellence**. However, it is different in multi-supplier, multi-vendor, system integrator, and IT consulting environments, where test automation scope, requirements, tools etc. are identified during the bespoke solution planning, design, and development phases. Implementing test automation is often influenced by the cost, reusability, post-live support, and internal/external stakeholder priorities. Therefore, managing these factors becomes the primary focus for managers and test leads prior to commencement of test approach.

The matrix in the below figure explains how stakeholders are to be involved based on their stake in the solution along with their interest in the solution.

Figure 1.4 Stakeholder involvement matrix

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-4.png)

Below is a set of factors to consider in managing both the internal and external stakeholders in the test automation process.

- Stakeholder identification. Identify all the stakeholders at the beginning. **Stakeholders fall into different categories such as business, IT and technology, legal, project management, suppliers and trusted partners, product or project team, infrastructure and environment team, or tool vendors**. It is important to work well with all these stakeholders for the success of test automation. For example, tool vendors and open source tool communities are an integral part of the success of test automation as they often provide timely support or professional services when the automation team faces technical challenges.

Note that some of these external stakeholders may be professional services that incur additional costs.

- The role of the stakeholders and their support to test automation vary based on their stake in the automation. For example, a business stakeholder may be the right person to provide test data for automated testing and an IT stakeholder may provide the right support for a test environment for automated testing, such as providing the infrastructure for automation, granting access to the servers, designing and building environments, and backing up the data. All stakeholders must agree and be clear on their role and responsibilities, and clarify their priorities.
- The below figure represents the stakeholders involved in test automation. The key stakeholders have a direct impact and are usually the primary beneficiaries of the solution; hence they are the centre of the stakeholder landscape. Other stakeholder support is required to deliver a successful solution and test automation.

Figure 1.5 Stakeholders

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-5.png)

- Goals. All projects have many priorities; however, stakeholders have their individual objectives and goals. It is vital to get an understanding of the key objectives of the stakeholders to plan how best to manage them. A good understanding of the key priority of the prime sponsor helps to define the automation approach accordingly.
  
  The rationale for stakeholder goals and business priorities regarding test automation generally fall into one of the following:
  
  - Complete the product or project implementation within the timeframe.
  - Being first to market to get an edge on the competition (reduce the testing window).
  - Cost reduction or controlling the cost.
  - Long-term return on automation investment.
  - Team reduction (e.g. reducing the number of manual testers).
  - Reuse of the existing automation tool licence and avoid procuring new tools.
  - Build automation capability internally and avoid external support.
  - Consistent and stable regression testing to increase confidence in releases.

A leading global provider of agricultural science and technology, in particular seeds and crop protection products, hired a global UAT test manager for a compensation management system that was implemented in over 90 countries. The UAT manager was on-boarded in August. Following a series of meetings with various IT and business leaders, the test manager listed the business, human resources (HR), data and IT objectives. After walking through the top three priorities in the meeting with the **chief technology officer (CTO)** of this European multinational agro company, it was understood that the primary priority of the key stakeholder (CTO) was to ensure that the tool would be available for production in December (timeframe) to adhere with the business needs for the next year. Any delay would impact the annual performance appraisal and the tool would not be useful for another 12 months, with the manual system continuing to fulfil the need for the current calendar year.

The testing scope and objectives were immediately reviewed and reprioritised to meet the key stakeholder’s goal.

- Communication. Communication channels, frequency and methods are to be defined and agreed upon with the stakeholders at the start of the product or project implementation. **Stakeholder communication should be value-based and differentiated based on their stake, that is, avoid the one-for-all approach to stakeholders**. For example, when providing periodic reports to the stakeholders, senior stakeholders may be interested to see the ‘traffic light’ or **red, amber and green (RAG)** report with highlights, and product or project stakeholders may be more interested in details of the test automation progress.
- Stakeholder engagement. It is important to **engage the stakeholders throughout the test automation as they will have a special interest in how it is shaping up**. Keeping them in the dark and ignoring their concerns will reduce or stop their buy-in. There should be no element of surprise for any stakeholder on a given day.
- Agree on the outcome. **Agree with the stakeholders on what is expected to be achieved, what are the benefits and return on investment, and provide evidence that the test automation is on track to achieving them**. Any change in plan or delay in achieving benefits should be communicated on time.
- Avoid overselling. **Avoid overselling and providing inflated benefits of test automation to the stakeholder to procure budget**. For example, avoid overselling or inflating the benefits of the test automation tools to justify the tool costs.
- Consult and consult again. The benefits of test automation, particularly in the early stages, may be unclear to its stakeholders. **Regular stakeholder consultation is essential to ensure that requirements are delivered to agreement**.

1.5 TEST AUTOMATION POLICY, STRATEGY AND PLAN

Test automation policy, strategy, plan and approach ensure test automation is designed and implemented as agreed. This is a key success factor in test automation.

**A policy is a document described at the organisation level and provides insight for the activities at the highest level**. The purpose of test policy and test automation policy is to **ensure that adequate direction is provided to all parts of the organisation, and associated third parties, in relation to testing and test automation**. The policy also outlines the standards required when performing software testing and test automation.

**Test automation policy, test strategy and test plan can be separate, stand-alone documents or a combined document, subject to the size of the organisation and practice**.

The document hierarchy of stand-alone documents is represented in the below figure.

Figure 1.6 Document hierarchy

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-6.png)

1.5.1 Test automation policy

A policy is **a statement of intent and is generally adopted by a governance body within an organisation**. Test automation policy provides guidance to **ensure the industry standards and the best practices in test automation are followed to achieve the most efficient and effective outcome**. Every test organisation and organisation that undertakes software testing (tech product and project-focused organisations) should have a test automation policy, which should adopt some of the key principles below:

- Test automation activities are carried out with proper governance and control.
- Test automation complies with test process maturity models.
- Test automation follows coding standards and guidelines.
- ROI should be calculated for all test automation activities.
- Automation feasibility analysis should be conducted for all test automation.
- **Cost-benefit analysis (CBA)** on automated testing should be performed before a test automation approach is concluded.
- Automated testing should be deployed as much as possible where the benefit of cost saving can be realised.
- Test automation should be used to maximise productivity and cost efficiency.

1.5.2 Automation test strategy

The test strategy is **a document describing the approach to the testing of the artefacts and is the top-level plan generated and used by the testing team to direct the test effort**. Test automation strategy **describes ‘what’ the test automation is for the solution and ‘why’ test automation is required**. It provides a summary of the test automation and responsibilities specific to the life cycle of the automation. It may be high level, dependent upon the availability of test automation requirements, and could further be elaborated in the following document, that is, the test automation plan. **Test automation objectives, scope and resources will be detailed** within the strategy document.

The purpose of a test automation strategy is to provide a rational deduction from high-level organisational objectives to actual test activities.

The main content of the automation test strategy is as follows:

- Purpose of the document
- Solution information and background
- The scope of test automation and why it is required
- High-level automation approach
- Test automation tool approach
  - Tool selection approach
  - **Proof of concept (PoC)** approach
  - **Proof of technology (PoT)** approach
- Phases of automation
- Test automation framework (high level)
- Environment details (high level)
- Roles and responsibilities
- Stakeholders that will be **responsible, accountable, consulted and informed (RACI)**
- **Risks, assumptions, issues and dependencies (RAID)**

1.5.3 Automation test plan and approach

The test plan **comprises separate documents for each test phase or a master test plan with all the phases and subprocesses in line with the test strategy, including all the information necessary to plan and control the test effort for the solution development phase**. It describes the approach to the testing of the artefacts and is the top-level plan generated and used by managers or leads to drive the test effort.

The automation test plan **describes the scope, approach, resources and schedule of intended test automation activities** (for example functional test automation plan or performance test automation plan). The test automation strategy explains the ‘whats’ and ‘whys’ of test automation, and the test automation plan **describes the ‘hows’ and ‘whens’ of automation, mainly about how and when the solution will be automated and executed**. It also identifies, among other test items, features to be automated, automation tasks, the task owner, test environment, test automation techniques, coding standards, and entry and exit criteria to be used. It is a document of the test planning process. This is **a living document of how test automation is to be implemented in a product or project, updated often to ensure that the plan and approach are up to date**.

The test automation plan **consists of an approach that is the implementation of the automated tests for a specific solution**.

The main content of the automation test plan is as follows:

- Purpose of the document
- Solution information
- High-level scope of automation
- How and when automation is performed
- Detailed automation approach
- Details of the selected tool
- Phases of automation implementation
  - Initial
  - Preparation
  - Final
- Test automation framework (detailed)
  - File structure
  - Features
  - Libraries
  - Reporting
- Guidelines and standards
- Test environments and data
- Stakeholders that will be RACI
- RAID

The sequence of activities and deliverables in the test automation approach are represented in the below figure.

Figure 1.7 Automation test approach

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-7.png)

1.6 CBA AND ROI FOR TEST AUTOMATION

Test automation has various impacts on many areas of software testing. It can save costs and resources while also resolving many testing-related problems. But there are many horror stories where test automation has failed and large investments have been shelved, causing customer dissatisfaction and ultimately calling off the automated testing. **Understanding cost versus benefits and computing ROI for test automation will help the leadership team in deciding to invest in automation tools for testing**. CBA is one way to do the ROI calculation.

1.6.1 Cost-benefit analysis

CBA is **a relatively simple and widely used technique for deciding whether to make an investment in test automation**. As its name suggests, simply add up the value of the benefits and subtract the costs associated with it. The automation costs are described in more detail later in this chapter. **Costs can either be one-off or ongoing**. Benefits are most often received over time. The standard justification for choosing test automation over manual testing is that the benefits exceed the costs over the life cycle of the product or project. Doing an actual analysis of the benefits and costs can encourage better decision making and ensure that resources are allocated effectively to support test automation.

A cost-benefit analysis is the **process to measure the benefits of a decision or an investment minus the costs associated with that decision or investment**. CBA is widely used for business and investment decision making.

The CBA should start during the planning phase (before implementation) for any project. As the requirements develop, we should be able to determine testing methodologies or techniques and start to develop the test plan and strategy. This early outline will be helpful to define and calculate the automation strategy and CBA. The testing leadership is responsible for ensuring that the CBA is executed for the automation. The lead should have expertise in automated test development in all the areas required for a CBA.

There are many factors to be considered when planning for a software test automation and analysis of cost and benefits. Automation changes the complexion of testing from design through implementation, test execution and test result analysis. The development, maintenance and execution of automated tests are quite different from manual tests. The skills, test approaches and, moreover, testing itself change when automation is practised. These impacts have positive and negative components that must be considered before performing CBA.

The major factors that should be considered for CBA for test automation are as follows:

- **Project specifications or product requirements** – The requirements are major factors to be considered for CBA. For example, the products designed for large user bases or multiple releases can impact the test automation approach and related benefits. A product based on a set of complex requirements may be difficult to automate, and it may incur long-term maintenance cost.
- **Functionality to be tested** – The functional and non-functional features. Some functionalities may not require any testing. For example, a **commercial off-the-shelf (COTS)** product may require minimum testing compared to a custom developed product.
- **Iteration or release of the software solution and testing** – A product that requires multiple iterations in the future can be a suitable candidate for automated regression testing and provide a high return in the long run.
- **Software testing and testing methodologies** – Costs and benefits of these are influenced by the software development life cycle. A DevOps-based product development requires frequent testing in multiple environments, and manual testing may not be feasible or incur a high cost.
- **Payback for the automation investment** – This is a key factor for CBA calculation. The payback is estimated based on many assumptions, and it needs to be revisited if any of the corresponding assumptions are changed.
- **Schedule variance and performance impacts** in testing when automation is introduced.
- **Future iterations of the SUT** – The number of future iterations with the life cycle of the SUT and amount of testing.
- **Tool patches, updates and so on** – Tool patches, patching windows, frequency and professional support for patching are major factors to be considered.
- **Resources available (e.g. hardware, tools, people)** – The resources required for any kind of testing need to be considered for CBA. It is important that the right resources be available for estimating CBA.
- **Reusability of previous test structures** – This can reduce the cost while increasing the benefits. However, previous structures can incur additional maintenance costs.
- **Test strategy and plan** – The test strategy and plan will provide an indication of the level and type of testing required for the solution in its life cycle.
- **Automated scripts maintenance** – This is a largely ignored area in test automation. The automated test scripts require changes subject to SUT changes, enhancements or new releases of the testing tool and so on.

CBA framework

The first step in performing a CBA is to define what you are testing and what you plan to automate. This will invariably come from the product or project plan and test plan as well as previous automation effort.

The below figure explains the CBA framework. **Benefits are estimated based on tangible and intangible factors**, and they can be impacted by the risks and assumptions. The testing can be performed manually or by automation or a mix of both. The work breakdown structure is generally used to further clarify the potential structures. Detailed data must be collected for each potential structure to estimate costs and benefits. Some possible sources of data are product knowledge, past projects, domain knowledge, current automation costs and online whitepapers.

The steps for a high-level CBA framework, which are explained in detail in the following sections, are:

1. Identify potential test structures
2. Ascertain assumptions and risks
3. Estimate benefits: tangible and intangible benefits
4. Estimate costs
5. Convert the costs and benefits into comparable values
6. Compare the alternatives and decision making

Figure 1.8 Cost-benefit analysis framework

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-8.png)

Identify potential structures The standard justification for choosing one level of testing over another is that the benefits exceed the costs over the life cycle of the project. Doing an analysis of the benefits and costs of using various testing structures can encourage better decision making. There are three different structures that should be considered when performing a CBA, and the one chosen should be the most cost-effective within the context of budgetary and timeline considerations. The structures are:

1. Automated testing (only automation)
2. Manual testing + automated testing
3. Manual testing (only manual)

When comparing structures, it should be ensured that the same level of test coverage has been considered for all structures. At this point, some structures can be rejected because they are not feasible.

Ascertain assumptions and risks As we are analysing these structures, we will be making a lot of assumptions, and there will be risks. It is important to identify the assumptions and validate them on the basis of fact or prior experience. For example we may assume that there will be one operating system and three service or security packs to this version of the SUT. Based on our track records and data, we will decide whether feasibility and maintainability will be an issue. This also provides a platform to explain why some structures were dropped in the analysis. If we did consider and eliminate some structures early on because of a conclusion that would not be feasible, the assumptions behind that conclusion should be clearly explained and justified.

Estimate benefits The benefits of any automation can be tangible or intangible. They are often mixed and sometimes difficult to measure. It is important to assess tangible and intangible benefits and assign a value or weightage to them. This can be positive such as cost reduction and quick testing. Likely tangible and intangible benefits are listed below.

Tangible benefits:

- Human involvement – Automated tests can reduce human involvement during testing, saving time, rather than manually running the same tests.
- Code coverage – Code coverage can be used to estimate test effectiveness. Automated tests can be incredibly effective, giving more coverage and visibility into the functionality of the SUT, for example testing an SUT for a large set of data.
- Test execution time – Automated tests can reduce the test execution time as computers are often quicker than humans.
- After-hours testing of systems – Automated testing helps to run the tests 24/7.
- There is a reduction in manual testing time for the current iteration and for future iterations.
- Automation of testing that would otherwise be impossible, for example load testing.

Intangible benefits:

Intangible benefits are difficult to assess but are a key factor for CBA and are generally intertwined with tangible benefits.

- Hands-off testing – Although the reduction in the cost of people is easily measurable, any additional value of saving in computer usage is difficult to quantify and is an intangible benefit.
- Good reputation of test organisation – This often increases the productivity of testing as the reputed test organisations have a high acceptance for their approach, established standards, rich in-house expertise and reusable **test automation solutions (TASs)** in order to assist the test automation.
- People – Not all members of the test team will want to change. Some turnover in personnel often accompanies test automation, even when some testers prefer to continue to test manually.
- Change in quality – The quality can be better after automation as automated testing can improve test coverage and consistency.
- Number of cycles of test execution – Automation often allows faster confirmation of product builds and provides the additional opportunity for the organisation to run the same test more frequently. This may not be feasible for manual testing.
- Payback – There can be unexpected payback from automation over a long period such as quick releases and reduction in testing cost. An immediate payback may be seen for some automation, for example build validation tests, but usually, some payback comes much later after the investment.
- Increase in reliability – Automated testing can be more reliable as it can avoid human errors due to the boredom of running the same test again and again. People are different, and the quality of manual test execution is dependent on individual capabilities.
- Satisfied customer – The test evidence from automated testing is more consistent and reliable. This can increase internal and external customer satisfaction.

Estimate costs Financial costs associated with automated testing can be generally described as either fixed or variable costs. Fixed costs of automation are expenditures for equipment, tools, training and so on. The variable cost increases or decreases based upon the number of tests that are developed or the number of times the tests are run. The following factors will be helpful in addressing the costs:

- Automated tests may generate mountains of results that can need much more staff involvement for analysis, thus costing more to run than manual tests.
- Time for automation planning, development and execution.
- Personnel cost is a key factor for automation costs. People with prior experience in automated testing are required for successful test automation, and experienced personnel increase the overall cost of testing.
- Hardware resource cost such as infrastructure required for tool installation, execution, configuration management and test execution machines.
- Testware such as software licences or software support such as professional support from the community and tool vendors.
- Automation environment maintenance such as test automation script backup.
- Tool introduction, training and ramp-up such as training from the vendor, training on programming languages and cost of certification.
- Test execution costs such as how often automated tests can be run, resources required for execution, result analysis and licence cost for execution.

In some cases, data may not be available to provide an adequate cost estimate. In that situation, the best alternative is to use the judgement and previous experience of the team members to estimate costs.

Convert the costs and benefits into comparable values After the costs and benefits for each structure alternative have been estimated, you will have a mixture of tangible (monetary) values and subjective level of benefit. It is generally harder to assign the benefits a financial amount. If there is no realistic way to relate the value of the intangible benefits to the tangible ones, they cannot be considered significant for the cost analysis. In this case, they can be used as a decision maker if the comparison of structures does not show that one structure is a clear winner. The effort should be converted to **level of effort (LOE)** and a monetary values assigned to it.

Compare the alternatives At this point, the analysis can proceed by comparing the net benefit (benefits minus costs) for each structure to determine which structure is best for the current project. The options with the greatest net benefit should be selected.

1.6.2 Return on investment calculation

In general, automated testing involves higher up-front costs than manual testing. Performing ROI analysis for test automation will help to determine up front what types of automation are ideal for the project, what tools will be required and what level of skill will be required for the testing. Not only does ROI serve as a justification for effort, but it is also a necessary piece of the planning process for the project. Projects that do not perform ROI calculations up front do not fully understand the costs of their automation effort, what types of automation they could be doing versus what they are doing, and what strategies to follow to maximise their return. The ROI is perhaps the single most effective way to garner the interest of decision makers. If you have compelling numbers backed by solid facts, and if you can show that every pound spent on test automation will return two pounds down the road, for example, then you are practically guaranteed funding.

Return on investment is a ratio between net income and investment. ROI is widely used to choose investment options. ROI measures the amount of return on a particular investment.

The ROI of test automation over releases is presented in the below figure.

Figure 1.9 ROI versus releases

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig1-9.png)

When it comes to automating the test process, the costs are tangible. But the net present value also includes many intangible factors (as we have already discussed in CBA). The findings in CBA can be used for an ROI calculation. The best approach is to determine the benefits with as much precision as possible and then compare them to the cost of automating the test effort.

A few different formulas to calculate ROI are:

1. ROI = Return/Investment
2. ROI = What you get out/What you put in
3. ROI = (Benefit − Cost)/Cost
4. ROI for automation = Benefits from automation over manual/Cost of automation over manual
5. ROI for automation = Cost of automation − Cost of manual testing

ROI calculation from the insurance industry based on formula 5

Business purpose: verify the functionality and validation of the base system for entering life insurance policies.

Cost of automation = Cost of hardware + Cost of software + Cost of test preparation, that is Test script development + (Test scripts maintenance x number of times scripts are executed) + Cost of test execution (Test script execution x number of times scripts are executed) + Cost of test result analysis + Defect reporting and tracking.

Cost of automation = £XXX.XX

Cost of manual testing = Cost of test preparation, that is Test case development + (Test case maintenance x number of times tests are executed) + Cost of test case execution, that is Test case execution x number of times tests are executed + Test result analysis + Cost of defect reporting and tracking.

Cost of manual testing = £YYY.YY

ROI for automation = Cost of manual testing − Cost of automation (£YYY.YY − £XXX.XX).

Note: A positive value shows there is positive ROI for test automation.

1.7 AUTOMATION FEASIBILITY

The organisation decides to progress the wide adoption of automated testing once the CBA and ROI are deemed reasonable. To achieve the best test efficiency, automation will be considered during the solution planning. The above analysis on automated testing should be carried out and presented to the stakeholders for approval on the investment. However, it is recommended that each team looks into its solution for automation suitability as not all solutions are suited for automation. This will help the organisation and the individual solution to use automated testing to reduce the cost of testing and improve efficiency. Automation suitability study at an individual product level will help the team to assess whether testing activities such as test case design, test data setup and test execution are suitable for automation.

The following factors are considered for automation feasibility or suitability analysis:

- Solution platform – A solution or product development for multiple platforms such as browsers, operating systems or environments will be highly suitable for automated functional and regression testing. However, the automation suite should be independent of platforms.
- Frequency with which the SUT code changes and is released – It is a good indicator for automation feasibility if the products require frequent testing. However, the automated pack requires frequent maintenance due to changes in the SUT.
- Tools availability and compliance – Availability of the SUT compliance tool is a key factor to be considered for automation feasibility. Lack of an automation tool will increase the effort and cost to develop an automation suite for testing.
- PoC or PoT – Proof of concept and proof of technology will help to understand the suitability of the SUT for automation.
- Resource availability – Availability of hardware, software and human resources is another key factor for automation feasibility.
- Benefit realisation – CBA supports benefit realisation for test automation.
- Duration of test execution – Automation may help to reduce the long manual execution cycle.
- Execution frequency – Frequently executed tests score high weightage in automation feasibility analysis.
- Technical complexity – Technically complex SUT and testing tools tend to increase the effort for automation.
- Live solution duration – The life cycle of the application is another factor for feasibility analysis. A SUT with long life is a good candidate for test automation and qualifies for feasibility analysis.
- Test data availability – Availability of test data for execution and less manual intervention to feed the data for testing will increase the weightage for feasibility.
- Dedicated environment for test automation – This provides a test environment available for automated testing and reduces the dependency on other teams.
- Requirement stability – Stable requirements will reduce the effort for automation.
- Detailed manual test steps – Detailed manual test steps reduce the effort for test automation preparation.
- Business as usual (BAU) team availability for handover – A dedicated post-live support team is a major factor for test automation. Lack of a support team will make the automated suite obsolete.



1.8 OVERSELLING AUTOMATION

One of the key problems in test automation is overselling to senior leadership. Over-projected stories from automation tool vendors and inflated success stories from other organisations presented to senior leadership can be detrimental later in the cycle.

‘Many organisations have not been able to get the level of Return on Investment from automation initiatives they would have wished for’ according to the World Quality Report 2019–20 (Capgemini, 2019).

In a rush to automate the solution and secure the investment, test automation is often oversold to the stakeholders. Overselling can have a negative impact on the success of implementing test automation across the organisation. This raises doubts in the stakeholders’ minds, and they may no longer trust the decision-making ability of the test managers. The common pitches used to oversell test automation are:

- Once test automation is achieved, testers will not be needed.
- One hundred per cent of automation can be achieved.
- Test automation should be implemented to meet the tight deadlines.
- If your automated suite is passing at 100 per cent, there are no defects in the application.
- High and quick ROI.
- It requires a single click to execute test cases through automation.
- Test automation will help to find more defects.
- Automated testing is always better than manual testing.

1.9 SUMMARY

Test automation is a subset of software testing, and it increases test coverage and supports a large volume of data testing. However, there are numerous challenges and complexities in test automation and, without overcoming them, it will be difficult to build and manage a successful automation function.

In this important opening chapter, we addressed what test automation is and why it is important in testing and product or project management. We also covered the decision factors in test automation and the advantages of automated testing over manual testing. This chapter also covered the importance of ROI and CBA in test automation and how to calculate them. Additionally, we addressed stakeholder management in test automation. Next, we will further uncover how test automation works in different IT business models, domains, testing types and testing stages.
