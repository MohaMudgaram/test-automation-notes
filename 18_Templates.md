## TEMPLATES

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

This appendix provides sample templates and structures, which need to be customised for your organisation. Each section of the table of contents needs to be expanded based on your specific requirements and may be different for your organisation.

TEMPLATE 1: SAMPLE TEST POLICY

Table of contents

1.Purpose

2.Scope

3.Definitions

4.Policy

4.1Risk-based testing

4.2Test artefacts

4.3Automated testing

4.4Maintenance

4.5Regression testing

4.6Requirements (all types)

4.7Test early

4.8Non-functional testing

4.9Test deliverables

4.10Resource skill sets

4.11Reporting

4.12Test metrics, KPIs and measures

4.13Test traceability

4.14Test governance

4.15Lessons learnt

4.16Software testing standards compliance

4.17Test tools

4.18Exceptions

1. Purpose

This policy is to ensure the following:

- Test activities are performed with governance and control, and comply with defined test processes.

- Test approaches are consistent and measurable.

- Risk-based testing is utilised on all projects.

- Where applicable, automated testing is considered, implemented and maintained to maximise test efficiency and cost savings.

- A proactive test approach is taken to ensure maximum productivity and to lower test activity costs.
2. Scope

This test policy will apply to all IT led programmes.

3. Definitions

IT: information technology

IT stakeholders: accountable domain leads, senior project leaders, project leaders, domain senior test managers, and test managers or leaders within or representing IT and business

4. Policy

Test policy is based on industry best practices such as ISTQB and PRINCE2.

- Risk-based testing – Risk shall be set during a number of workshops with all key stakeholders to ascertain the test risk of the requirements, features and functions within the project. Requirement risk analysis can still be conducted if the project deems it necessary, and this will be performed using industry standard best practices within the test management tool.
- Test artefacts – All test artefacts such as test plans, test scripts, frameworks, test data and defects will be created and maintained throughout the life cycle.
- Automated testing – All IT programmes and products should complete an automated testing feasibility study using the predefined automated testing feasibility template or tool. The tool contains a set of questions around the software solution and the long-term impact.
- Maintenance – All automated test suites or packages must be maintained; the test manager is responsible for ensuring that the automated testing is handed over to service run/BAU team and maintained for future use.
- Regression testing – All regression testing is expected to be automated unless the automation suitability checklist identifies that there is insufficient return on investment (ROI).
- Requirements – Before testing activities start the requirements must be signed off. Once the requirements are in the test management tool and tests are linked to the requirements, then all further requirement updates must be performed within the test management tool. This ensures all changes are tracked and the audit trail is in place. Requirement test coverage of 100 per cent will be achieved unless there is prior agreement with the project stakeholders due to descoped requirements, in which case the requirements will be marked accordingly but will remain within the test management tool.
- Test early – Early life cycle testing must be adopted.
- Non-functional testing – Non-functional testing should include performance, load, stress, capacity, IT service continuity (ITSC) and security testing. The results of all non-functional testing must be stored within the test management tool, to demonstrate full coverage, risk and direct cover status.
- Test deliverables – All test deliverables must be available at any time to be reviewed and audited.
- Resource skill sets – All resources involved in any aspect of testing must have sufficient test skills to fulfil the role. They should have good domain knowledge and understanding of the business processes of the system under test.
- Reporting – Reporting will occur during the complete life cycle to ensure that there is a clear prediction of completion date, coverage and risks. All status reports must be generated from the test management tool. The reports are to include requirement coverage, direct cover status, defect logging, test write progress, and test execution status against releases and cycles.
- Test metrics, KPIs and measures – Project level performance metrics and measures will be captured throughout the project.
- Test traceability – All test activities must be included in the overall project plan and should be accessible.
- Test governance – All programmes must have a single point of accountability for the overall delivery of all test activities on the project to ensure consistency and that testing is efficient and cost-effective.
- Lessons learnt – Upon the completion of a project, project teams should take part in a test-focused lessons learnt session to establish where test efficiencies can be improved, costs reduced and risks mitigated for future projects.
- Software testing standards compliance – All testing activities should comply with ISO/IEC/IEEE 29119 software testing standards and those outlined in the test policy document.
- Test tools – This section lists tool selection.
- Exceptions – Any exception must be made with deliberate consideration of all the associated risks, and exceptions must be agreed with the stakeholders.

TEMPLATE 2: SAMPLE TEST AUTOMATION PLAN

Table of contents

1.Document control

1.1Document information

1.2Version history

1.3Distribution list

1.4Approvals

1.5Source documents

2.Introduction

3.Test scope

3.1Activities

3.2Entry and exit criteria

3.3Deliverables

3.4Test approach

3.5Governance

4.Test automation

4.1Testing techniques

4.2Testing tools

4.3Suspension and resumption criteria

5.Test automation framework approach

5.1Approach

5.2Test data

5.3Execution flow

5.4Test preparation

5.5Test environment

5.6Automation test execution

5.7Automation test management

5.8Automation test schedule

6.Test metrics

7.Risks, assumptions, issues and dependencies

8.Responsible, accountable, consulted and informed matrix

1. Document control

1.1 Document information

1.2 Version history

This document is subject to change control after it has been formally signed off. All subsequent changes to this document must adhere to the document control process and change management process.

1.3 Distribution list

1.4 Approvals

1.5 Source documents

The inputs for this document have been based on, or should be read in conjunction with, the following documents:

- Document 1 (example)

- Document 2 (example)

- Document 3 (example)
2. Introduction

This document is the automation test plan for the project. This test plan includes the objective of test automation, which is to determine whether the functionality of the system under test is as per the requirements. The objective of automation is to automate test scenarios and test cases that are common functionalities across various modules undergoing the project implementation. The same test suite can be executed to perform a regression test run without investing time and effort. The intended audience of the automation test plan document includes the project manager, QA manager and entire functional testing team and development/solution teams.

3. Test scope

3.1 Activities

|                          |                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Area                     | In scope and out of scope                                                                                                                                                                                                                                                                                                                                                                                              |
| Feasibility and planning | Analyse the functional test cases for automation regression testingIdentify the test cases for automation; prepare the automation planIdentify the repetitive tasks and create the test automation frameworkIdentify relatively stable areas of the application over volatile ones for automationThe common workflows to be performed by the end-user will be automated first                                          |
| Test case automation     | System under test: [Name]Web application will be automated using [Tool name]Automation feasible test case count: [Number]Tool: [Tool name] with [Programming language name] as programming languageFramework: Hybrid-based framework will be used for automationLanguage versions: Application version – EnglishDelivery plan: The automation will be delivered with the below number of test cases that will automate |
| Business scope           | Areas of application that have least priority for the business will be out of scope                                                                                                                                                                                                                                                                                                                                    |
| Test automation          | Areas of application for which there is no functional or technical reference present in the requirements document                                                                                                                                                                                                                                                                                                      |

3.2 Entry and exit criteria

Entry criteria:

- Functional test plan and test cases – reviewed and signed off
- Application build with proper release notes from the development team
- Test data required for the test
- Environment setup (e.g. UFT installation and integration with ALM)
- All the available system set up (OS machine and devices)
- Application knowledge transition

Exit criteria:

- All the feasible test cases have been automated.
- The customer has signed off on the automated test cases and automated testing scope.

3.3 Deliverables

- Automation test plan
- Automation test scripts
- Automation test execution summary report

3.4 Test approach

The focus of the test automation is to automate the steps used for testing the application manually. It will be designed based on the functional test scenario identified and thus verify the crucial functional units. The test automation team will utilise a data-driven approach to test, analyse and validate the application.

The test automation consists of the following high-level activities:

- Identify high-level test scenarios.
- Identify the reusable components.
- Create a design document for the identified reusable components and specific scripts.
- Set up the data for test automation.
- Develop automation test scripts.
- Review automation test scripts.
- Execute automation test runs through test management tool.
- Carry out the defect analysis during the automation test execution phase.
- Report/track automation test defects.
- Report test summary results.

3.5 Governance

The QA responsibilities assigned are listed as follows:

- Create automation test plan.

- Estimation, planning and control.

- Obtain the sign off for automation test plan.

- Manual test scenarios and test scripts review.

- Automation test scenario and script review.

- Oversee test execution and defect management.

- Obtain the sign-off for test summary report.
4. Test automation

Test automation will involve automating the functional test scenario identified. The main objective of test automation is to validate the functionality of the application.

4.1 Testing techniques

The test automation team will utilise a data-driven approach to test, analyse and validate the SUT. The data-driven approach is applied for the test automation activity as it separates data from the automation scripts. This allows the features to be tested with a different set of input values and also by parameterisation of scripts, and scripts can be run on multiple data sets to verify that the application works as expected. It allows process flows to be tested first and then the end-to-end scenarios interacting with external systems will be tested. In future any change in data requires only the data set to be updated and not the automated script.

4.2 Testing tools (example)

|                                    |                                                    |
| ---------------------------------- | -------------------------------------------------- |
| Test process                       | Tools                                              |
| Test automation                    | - HP Unified Function Testing                      |
| Test management                    | - HP ALM                                           |
| Defect management                  | - HP ALM                                           |
| Test execution (scenarios/scripts) | - HP ALM and Unified Functional Testing (UFT)      |
| Test data creation                 | - HP UFT inbuilt MS Excel spreadsheet (data table) |

4.3 Suspension and resumption criteria

Testing can be suspended under the following circumstances:

- Connection issues with the automation tool licence server.
- Non-availability of system under test.
- Network fluctuations.
- Unresolved build errors.
- Unscheduled technical disruptions to the testing environments.

If a test case fails, testing will be suspended for all dependent features. The failed test case will be logged in a defect log along with a description of the failure.

Testing will resume, from the point at which it was suspended, when the items listed above are resolved.

If a full suspension occurs and can be pinpointed to a specific software release, then the re-deployment of the previous successful software release will be considered if further testing of that and earlier increments is thought to be of benefit.

5. Test automation framework approach

5.1 Approach

The approach section provides the solution test automation. At high level, the test automation life cycles are based on following industry standards.

The SUT automation will be carried out based on the above defined automation approach, methodology and the following framework. This automation approach and framework advocates the usage of data-driven testing within the industry standard methodology.

The framework consists of the following elements:

- Data-driven scripts
- Business components
- Application area
  - Object repository
  - Utility and generic functions
  - Reporting functions
- Automated test execution
  - Individual and batch execution
- Report manager
  - Excel reports
  - UFT standard reports

5.2 Test data

The test data will be created according to the parameterisations done during the process of automation test script creation and will be maintained in the MS Excel spreadsheet. A separate MS Excel sheet will be maintained for each test script, it will contain the data set used by the script and will be stored in the test management tool. This will ease any changes that need to be made to the data set.

5.3 Execution flow

- All the libraries will be associated with runtime (loaded at runtime).
- The test automation script will read the business component tests mentioned in the process flow tab and execute them one by one.
- All the components mentioned in business library will be executed by the automation script.
- The report will be generated in MS Excel and HTML formats.

5.4 Test preparation

The following test preparation activities are required:

- Verify connectivity between the automation tool and licence server.
- Confirm test management tool and automation tool connectivity for storing the test script and execution.

5.5 Test environment

Testing is truly enabled by a system environment plan. The following points outline the code promotion path for the project:

- The automation team requires access to all the required tools.
- Test environment: functional and end-to-end (E2E).
- Database access to prepare the test data.

5.6 Automation test execution

Automation script execution will be carried out through the test management tool. Defects found during each cycle will be reported through the defect tracker. The team will record any defects using the defect management process defined. Automation test scripts will be re-executed to ensure that the bug fixes have not affected any other part of the application. As test execution progresses, the test governance lead will constantly update and modify the test execution matrix according to which test scripts have passed and failed, which cannot be run due to dependencies on other things, and which need to be retested because of failure or defects.

A test summary report will be created that will contain information on the total number of test cases executed and defects found during each test cycle.

5.7 Automation test management

The following test management activities have been defined:

- Manage and control automation test life cycle.
- Manage the automation test scripts.
- Perform automation test execution.
- Investigate and resolve discrepancies.
- Prepare test results and defect reports.
- Review test results and defect lists.
- Create test summary report.
- Validate whether or not all testing tasks have been completed.
- Obtain sign-off.

5.8 Automation test schedule

The following are examples of a test automation schedule in two different formats.

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/f0211-01.png)

6. Test metrics

Accurate reporting of test results is just as critical as the actual testing itself. Effective test metrics provide test management ability to report progress of the test against plan in several ways. A baseline level of metrics should indicate planned and actual test execution results, as well as all active defects by status. More sophisticated metrics provide trend analysis and some outcome projection capabilities. The test team will create and communicate the metrics periodically.

7. Risks, assumptions, issues and dependencies (RAID)

8. Responsible, accountable, consulted and informed (RACI) matrix

TEMPLATE 3: COST-BENEFIT ANALYSIS

Factors to be considered:

- Total cost of the test automation versus 100 per cent manual testing.
- When will the full ROI be realised?
- What are potential risks or challenges?

Figure A.5 Tentative high-level plan and schedule

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/FigA-5.png)

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/img213.jpg)

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/img214.jpg)

TEMPLATE 4: AUTOMATION SUITABILITY CHECKLIST

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/f0214-01.png)

|                                         |
| --------------------------------------- |
| Key                                     |
| < 50%: Not ideally suited to automation |
| 50–60%: Automation is viable            |
| 60–75%: Suitable for automation         |
| > 75%: Great automation candidate       |

|                      |       |
| -------------------- | ----- |
| Area summary         | Value |
| Project %            |       |
| Ability to execute % |       |
| Test quality %       |       |
| Handover %           |       |
| Total %              |       |

|                                    |        |
| ---------------------------------- | ------ |
| Project suitability for automation | Yes/No |

TEMPLATE 5: TOOL EVALUATION

|                 |                    |
| --------------- | ------------------ |
| Tool evaluation |                    |
| Tool name       | [Name of the tool] |

|                                              |                                             |     |
| -------------------------------------------- | ------------------------------------------- | --- |
| Vendor/community                             | Vendor/community support                    |     |
| Vendor size                                  |                                             |     |
| Vendor support available                     |                                             |     |
| Vendor refund policy                         |                                             |     |
| Any initial training by vendor               |                                             |     |
| Costs                                        | Is this a licenced or open-source tool?     |     |
| Purchase costs                               |                                             |     |
| Support costs                                |                                             |     |
| Maintenance costs                            |                                             |     |
| Type of licences                             |                                             |     |
| Skills                                       | Are the staff skilled in tool usage?        |     |
| Does the tool require development knowledge? |                                             |     |
| What coding language knowledge is required?  |                                             |     |
| Project use                                  | Does the tool support the technology stack? |     |
| Single product use? Or multiple projects?    |                                             |     |
| Integration                                  | Integration with test management tool       |     |
| Import/export capability                     |                                             |     |

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/f0216-01.png)

TEMPLATE 6: ROI TREND

|                                            |        |
| ------------------------------------------ | ------ |
| Regression testing scope                   |        |
| Approximate total no. of test cases        | 414    |
| Automation %                               | 75%    |
| Approximate test cases in automation scope | 316    |
| Approximate test execution cycles in year  | 5 to 6 |

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/f0216-02.png)

|                                       |        |            |
| ------------------------------------- | ------ | ---------- |
| Total effort for given cycle in hours |        |            |
| Cycles                                | Manual | Automation |
| Dev                                   | 1465   | 3330       |
| 1                                     | 2292   | 3738       |
| 2                                     | 3119   | 4107       |
| 3                                     | 3946   | 4433       |
| 4                                     | 4773   | 4759       |
| 5                                     | 5600   | 5085       |
| 6                                     | 6427   | 5411       |
| 7                                     | 7254   | 5737       |
| 8                                     | 8081   | 6063       |
| 9                                     | 8908   | 6389       |
| 10                                    | 9735   | 6715       |
| 11                                    | 10562  | 7041       |
| 12                                    | 11389  | 7367       |
| 13                                    | 12216  | 7693       |
| 14                                    | 13043  | 8019       |
| 15                                    | 13870  | 8345       |

Figure A.6 ROI chart for automation

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/FigA-6.png)

TEMPLATE 7: ROI

Benefits/value estimation:

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/f0218-01.png)

Cost estimation:

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/f0219-01.png)

Factors:

The questions and factors shown below should be carefully considered for the ROI calculation

|     |                                                                     |       |
| --- | ------------------------------------------------------------------- | ----- |
| No. | Factors                                                             | Check |
| 1   | How much time do you have for training?                             |       |
| 2   | What is the scope for test automation?                              |       |
| 3   | Do you want to establish traceability for compliance?               |       |
| 4   | Is it record and playback test automation?                          |       |
| 5   | Does the application support automation?                            |       |
| 6   | Does the testing tool support automation?                           |       |
| 7   | Does the SUT architecture and technology support automation?        |       |
| 8   | Does the application domain support automation?                     |       |
| 9   | Does the test case support automation?                              |       |
| 10  | What is the test coverage of automation?                            |       |
| 11  | Does it catch defects sooner in the software life cycle?            |       |
| 12  | Is the development of scripts a parallel effort to SUT development? |       |
| 13  | Does it bring value to the customer?                                |       |
| 14  | Does the project require automation?                                |       |
| 15  | Do you have a test automation strategy?                             |       |
