## DOMAIN-FOCUSED TEST AUTOMATION

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

Test automation is the validation of a software solution using other software. There are lots of failures in test automation, the main reason being the limited experience of test managers across various domains and sectors. Test automation itself is an IT project, and no two IT projects are the same. Many test automation projects end in failure as the team tries to replicate the automation success from a previous project to the current project without considering the various factors that are salient to the current engagement.

This chapter explains how test automation is applied across different domains, sectors and development approaches such as Agile, Waterfall, DevOps, continuous integration (CI), Lean, Kanban and so on. It aims to assist test managers, Scrum masters and automation leaders in understanding the challenges and factors to be assessed before commencing automation planning. In the following sections, test automation is further explained in different SDLC approaches, business models, testing stages or subprocesses, testing types and the latest trends in test automation.

The below table provides a synopsis of this chapter.

Table 2.1 Test automation and domains

|                                |                                                                                              |
| ------------------------------ | -------------------------------------------------------------------------------------------- |
| Domains                        | Area covered                                                                                 |
| SDLC or development approaches | Agile, Waterfall, DevOps, CI.                                                                |
| Business models                | IT consulting, project, product, MS/MV, SI, managed testing services (MTS), start-ups, SMEs. |
| Testing types                  | Functional and non-functional testing.                                                       |
| Testing subprocess (stages)    | System testing, integration testing, regression testing.                                     |
| Latest trends                  | Artificial intelligence (AI), machine learning (ML), robotic process automation (RPA).       |

2.1 SOFTWARE DEVELOPMENT APPROACHES

This section covers test automation in Waterfall and Agile software development approaches.

Software solutions are developed through different approaches, and most of them follow a flavour of either traditional Waterfall or Agile approaches. Test automation itself is an IT solution, and hence it should follow an approach. In most cases, test automation is part of a wider IT programme, and it follows the programme’s software development approach. However, many organisations consider test automation itself as an IT project, and this allows them to follow a development approach of their choice.

The software development process is a methodology that describes the activities involved in defining, building and implementing an IT system.

**The Waterfall testing approach follows the same structure as the Waterfall software development approach wherein there is a sequence of stages in which the output of each stage becomes the input for the next stage**. Testing is performed step-by-step in line with the implementation steps, subject to the completion of a phase or stage.

The below figure shows the different steps/stages of the Waterfall approach.

Figure 2.1 Waterfall approach

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-1.png)

**Agile testing is based on the Agile development approach, where testing is not a different phase and is performed alongside development phases that include requirements analysis, design, coding, test case development and automation**.

The below figure shows a pictorial representation of the Agile development and testing approach.

The Waterfall and Agile testing approaches are fundamentally different. The below table compares Waterfall and Agile testing.

Figure 2.2 Agile approach

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-2.png)

Table 2.2 Comparison between Waterfall and Agile testing

|                                                                                                                                      |                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------- |
| Waterfall testing                                                                                                                    | Agile testing                                                  |
| Testing is separate and in distinct phases, such as system testing, system integration testing, performance, volume testing and UAT. | Testing is not a separate phase or stage in Agile testing.     |
| Formal testing is performed only after the completion of development or a stage.                                                     | Testing is performed alongside the development.                |
| The development and testing teams work separately.                                                                                   | The development and testing teams work together.               |
| Testers may or may not be involved in the requirement definition.                                                                    | Testers are involved in requirement refinement and estimation. |
| Test automation is subject to project need.                                                                                          | Test automation is an essential part of Agile.                 |
| Acceptance testing is a separate stage and performed at the end.                                                                     | Acceptance testing is performed at the end of each iteration.  |
| Big teams involved.                                                                                                                  | Small team and more collaboration.                             |
| Regression testing is carried out only after defect fixes or releases.                                                               | Regression testing is carried out frequently.                  |
| Long-term planning.                                                                                                                  | Short-term planning.                                           |
| Distinct testing phases.                                                                                                             | Overlapped testing phases.                                     |
| Defined and structured implementation.                                                                                               | Flexible implementation.                                       |
| Majority of the testing is left to towards the end of development.                                                                   | Frequent testing throughout development.                       |

In the real world, many large projects are implemented using the hybrid approach, that is, Waterfall and Agile.

A large government department designed and implemented an intranet portal based on a Microsoft (MS) SharePoint-based cloud platform. The implementation team followed different development methodologies as appropriate. The SharePoint tool configuration, implementation, functional testing and test automation followed Agile-based development methodology. Infrastructure and non-functional testing used a more suitable Waterfall-based testing approach for the solution.

Functional testing was based on two weeks’ Sprint (Agile approach), including fully automated regression testing with Microsoft Team Foundation Server (TFS) and Azure DevOps toolsets. However, performance testing was based on the Waterfall approach fully agreed and signed off requirements using the Micro Focus LoadRunner tool.

The following sections cover test automation in Waterfall and Agile along with another popular approach, DevOps.

2.1.1 Test automation in Waterfall

The Waterfall approach consists of step-by-step phases, where each phase depends on the deliverables of the previous one. This approach is widely followed in large projects. Waterfall requires clear structure and documentation up front. It is divided into distinct stages or steps with quality gates to finish the current stage and start the next one. The stages are relatively standard and often follow a sequence: agree on the requirements and scope, design, implement, test, deploy and post-live maintenance. There is less flexibility with this approach; what is agreed at the beginning must be seen through. However, this approach reduces uncertainty and increases the ability to work on a clear scope and requirements. Changes are often addressed by the **change control (CC)** process, and it reduces the overall cost.

Test automation in Waterfall projects is easy to implement as the requirements, test cases and a stable application is available for automation.

Test automation and Waterfall characteristics:

- Application is available for a proof of concept for test automation – This reduces uncertainty and supports the tool selection and tool compliance for test automation.
- Quick to estimate and calculate ROI as the requirements are stable and agreed.
- Faster test automation as the application is available – An existing and stable application enhances test automation. A stable GUI is essential for GUI-based functional test automation, and it reduces the rework of test scripts.
- Scope and approach for test automation is clear – This allows test managers to plan and estimate test automation and reduces the uncertainty, as the requirements are agreed upon prior to test automation commencing.
- Cost of test automation is under control – The stable application, agreed requirements and scope help test automation deliver in line with the agreed plan. This reduces rework and cost and provides additional control in test automation implementation.

Figure 2.3 Waterfall testing

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-3.png)

Limitations of the waterfall approach in test automation:

- Requirement changes are difficult to manage – The Waterfall development approach and Waterfall-based test automation provide limited opportunity to absorb changes. The requirements are agreed upon prior to test automation commencing, and any changes to the requirements are often addressed through a CC process. This limits the opportunity to respond to the changes and feedback.
- Lack of flexibility – Waterfall is known as a structured process and lacks flexibility. Waterfall-based test automation starts after agreeing on the requirements, framework, architecture and schedule, and there is no or limited room for flexibility.
- Not usable for ongoing application development – Waterfall-based automation is not suitable for ongoing **continuous integration and continuous delivery (CI/CD)** and DevOps-based development as the test automation suite is not delivered frequently and not built to address ongoing development.
- Test automation commences only after application or functionality development – This reduces the ability to use the automation suite during the product development stage.
- No real-time use of ongoing testing, as automated testing commences only after the development is complete.

Figure 2.4 Test automation in Waterfall

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-4.png)

There is a leading scientific and technology software company, headquartered in the United States, with representation in Europe and Asia, providing software for chemical, material and bioscience research for the pharmaceutical, biotechnology, consumer-packaged goods, aerospace, energy and chemical industries. The products are highly scientific in nature, and requirements are agreed upon prior to implementation. The requirements are stable and require minimal changes during implementation.

The products are frequently regression tested in multiple cycles during development stages and post-release. The automated test suite is used for regression and release testing of migration, porting, web, stand-alone, client–server, product testing and cross-platform testing.

The automated regression suite is developed using the Waterfall development approach due to the nature of the applications and the stable requirements for testing and test automation. Due to the nature of the product, platform and release, the automation suite provides almost 100 per cent coverage on regression testing with minimal maintenance.

2.1.2 Test automation in Agile approach

The Agile development approach was developed as a response to growing frustrations with Waterfall and other highly structured, inflexible approaches. This approach was designed to accommodate changes and produce software quicker. Agile emphasises working as one team, customer collaboration throughout the development approach and focuses on creating working software rather than documentation. In the Agile approach, project teams develop the solution and a list of deliverables in short Sprints or iterations of 2–3 weeks in general, based on the business and technical priorities. During development, teams work towards the goal of delivering working software and review the progress, status and outcome of the deliverable at the end of the Sprint. This is a feedback-driven process and is well accepted by the business community. Agile is collaboration-focused and client satisfaction is the priority in the approach. However, Agile projects sometimes lack control when managing costs, requirements, scope and discipline, resulting in unsatisfied customers.

Agile test automation is an approach to using test automation in Agile development with the purpose of making testing more effective and in line with the Agile way of development. It reduces the dependency on manual testing, uses test automation to speed up the application development, reduces the manual testing effort and uses the team better. This approach accommodates changes. Agile automation aims to automate everything feasible and to replace manual testing rather than using automation for additional benefits. Many Agile test teams tend to automate the features of previous Sprints and use the automation test suite for continuous regression testing.

Test automation and Agile development characteristics:

- Test automation is parallel to product development – Many Agile teams tend to spend the first part of the iteration on requirement clarification, manual testing and so on, and the second part of the same iteration for automated testing. This allows the team to build good knowledge of the features, test them manually and ensure they are stable prior to test automation. This enables faster test automation and frequent execution.
- Agile automation supports ongoing product development by performing automated build validation, smoke testing and regression testing.
- Quick ROI and customer satisfaction as the result of test automation is immediate, within the same Sprint or iteration.
- There is high reusability and support of ongoing releases – The automated test suite is used time after time, mostly daily regression testing and build validation.
- There is high coverage on requirements and testing – Agile automation aims to automate everything feasible and provides high test coverage.
- Long-term costs are lowered by reducing the manual effort for frequent test execution.
- Solution and testing requirements are met quickly as the test automation is parallel to product implementation.

Testing is the core of Agile development and plays a significant role in the inception, construction and transition phases. Test automation enhances the development and testing in the Agile approach.

Figure 2.5 Agile testing

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-5.png)

Figure 2.6 Test automation in Agile at an enterprise level

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-6.png)

Limitations of the Agile approach in test automation:

- Focus is on getting test automation done in time when it is needed, and not how effective or efficient it is.
- Test automation tends to focus more on functional testing, and non-functional testing is often ignored.
- High maintenance, as automated test scripts require continuous maintenance in line with the Agile delivery.
- The application continually evolves, iteration after iteration, and therefore due to lack of a stable application, testing is difficult to automate.

A leading travel and transport provider implemented identity and access management (IAM) for their external customers who use multiple commercial applications. Customers used to register and maintain separate accounts to access each of the applications and services they are interested in. The IAM solution allows customers to use a single identity with associated personal details and preferences, providing access to a range of applications.

The implementation took a phased approach to the application of IAM and was delivered using a Disciplined Agile methodology. The product backlog contained requirements that were delivered through a number of user stories. The product backlog is a living set of requirements accountable to the product owner.

The **minimum viable/valuable product (MVP)** was defined during the inception and the solution was delivered over a few deployments. The product backlog and user stories that form the test basis were captured in the Microsoft Azure DevOps tool. Lightweight test plans were created for each iteration based on the user stories and acceptance criteria selected in that iteration backlog. Test cases were developed to validate the acceptance criteria of the user stories, enabling requirement traceability. Testing was based on the IAM architecture and Selenium was used for test automation. Regression testing was 100 per cent automated.

2.1.3 Test automation in DevOps

**DevOps is a set of practices that combine software development (Dev) and IT operations (Ops) together, thus the name ‘DevOps’, or ‘development operations’**. It aims to increase the rate of solution development with frequent releases utilising many practices from the Agile development approach and Lean principles.

DevOps is a set of tools and key practices that increase the ability to deliver applications at high velocity over traditional software development and infrastructure management processes such as Waterfall and Agile.

Test automation plays a key role in the success of DevOps and is inevitable.

In DevOps style, programmers and test automation engineers work together, supporting the test team in developing an automation framework to perform DevOps testing. The development team contributes to test script development as there is just a thin line of separation between developers and automation engineers. The automated scripts and codes are supported by CI/CD tools, generating builds automatically, deploying and testing them.

The scope, plan, pipeline and production release are defined in advance in order to plan and implement DevOps testing. There are many frameworks available for DevOps implementation and testing, such as Microsoft Azure DevOps Services, Amazon Web Services (AWS) Developer Tools and Google Cloud.

Figure 2.7 DevOps

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-7.png)

Figure 2.8 DevOps CI/CD workflow

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-8.png)

Test automation and DevOps characteristics:

- Code and configuration changes are continuously tested in DevOps. Test automation is the key to achieve this goal.
- Feedback loops are fast and detailed. The new features are continuously tested by the automation suite, and this provides immediate feedback on quality. Test automation shortens the lead time between fixes.
- Automated non-functional testing suites are part of the pipeline and run early in the cycle.
- Automated end-to-end functional testing integrates well with testing frameworks.
- Close association of the development and automated testing team leads to effective cross-functional teamwork and reduced resource dependencies.
- Test automation is a key focus area in DevOps, and it is essential to achieve DevOps goals. This lowers the failure rate of new releases to live and minimises disruption of releases.
- Speedy delivery, high flexibility and instant scalability of additional features and functionality as test automation enhances the testing efficiency and shortens the testing timeframe.

The list above covers a few common goals for both Agile and DevOps, although they are not achieved as often in Agile. However, DevOps gives more emphasis to ensure these goals are met.

The below figure explains the close association of developers, testers and automation SMEs in the DevOps model. They often interchange their roles in DevOps. A fully working test automation is a key success factor for DevOps.

Figure 2.9 DevOps test automation

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-9.png)

Limitations of DevOps in test automation:

- Continuous and frequent release to production is a core objective of DevOps. However, production rollback could be cumbersome and messy in a few instances.
- Continuous updates to the production system are not always feasible and are difficult for legacy code.
- High scripting and programming skills are essential for the success of DevOps. It requires heavy investment in tools and hardware.
- Mindset for cross-functional collaboration is essential for the success of DevOps, and any human intervention or conflict slows down delivery.
- DevOps is challenging in projects and in products with highly integrated environments, and continuous maintenance of test automation is required.
- Not suitable for highly regulated industries or secure sectors as any release to production requires auditing by the regulators, prior approval and so on.

A large European ‘digital retail’ organisation decided to build a set of tools that would enable the company to increase retail sales.

The programme features were:

- An online shopping site with minimal IT and marketing investment
- The development and test environments hosted within the cloud using a software as a service (SaaS) or infrastructure as a service (IaaS)
- The solution development followed a DevOps model

The following toolsets were considered to support the DevOps:

- Deployment – Jenkins, Puppet
- Continuous integration – Jenkins, Selenium
- Source control – GIT
- Development environment – Vagrant, Puppet
- Configuration management – Puppet, Ansible
- Monitoring – Azure Control Center, App Insights
- Issue/defect tracking – Visual Studio Team Services (VSTS) or Azure DevOps
- Planning – VSTS or Azure DevOps, Microsoft Project
- Collaboration – Confluence wiki, SharePoint

2.1.4 Continuous integration

CI is one of the original twelve practices of the extreme programming (XP) development process. XP is a software development methodology that was developed by Kent Beck. XP was one of the first Agile methods, as well as being the one that is predominantly used before Scrum takes the lead. CI is a software development approach where the work is integrated frequently. It is also a DevOps best practice and allows developers to frequently merge code changes into a central repository. The code merge or check-in is verified by an automated build and test, that ensures that problems are detected earlier. CI is a modern software development practice in which incremental code changes are made frequently and reliably.

The developers integrate their code at least daily, though often more frequently. The CIs are validated by automated tests with the intention of finding integration errors as quickly as possible. One of the key benefits of CI is that the automated build and test reduces integration problems and helps the team to develop and deploy the software more rapidly. The automated CI and CD improves code quality and thereby security.

A CI server such as ‘CruiseControl’ is useful for code deployment, as it builds a custom continuous build process, monitors the code changes, and alerts errors, even though CI does not require any tooling in order to be deployed. There are many on-premise, cloud, and hybrid tooling solutions available for CI that perform tests on every change and monitor the repository for changes. There are many licensed, procured, free, and open source CI automation servers such as Jenkins, TeamCity, GitLab CI, Bamboo, Buddy and so on, which are widely used for facilitating CI and CD to build, test, and deploy software.

Automation is a key activity in CI. The automated test suite validates the code changes and integration to the main and shared code repository. Performing automated tests on every branch helps identify issues early. Automated testing is key for the success of CI as the test automation suites provide immediate feedback to the developers on their product. The automation suites are generally split in two; the first set provides quick feedback (e.g. unit tests), while the second set provides more detailed test feedback. The first set of quick tests always helps the developers reduce the waiting time for the test result.

One key aspect of test automation in CI that the team needs to ensure is that the feature that gets developed has corresponding automated tests, and tests are upgraded in line with new releases, and regression issues. The developers need to be involved as early as possible in the definition of the user stories to create good tests. The test-driven development (TDD) is widely practiced in CI as the tests are created before writing the code that will fulfil the test.

The generic CI steps are as follows:

- Step 1. Create tests (e.g. TDD) for the key features of the solution and the codebase.
- Step 2. Run the tests automatically (e.g. using a CI server) on every code merge to the main repository.
- Step 3. Developers integrate code changes frequently or as soon as possible.
- Step 4. Fix errors and the CI build as soon as it is broken.
- Step 5. Write new tests to enhance the test base for new stories.

CI was initially created for Agile development. CI works well with the ‘Test Pyramid’ developed by Mike Cohn and implements test automation at various levels.

- Unit tests. Unit tests are performed at micro levels, which verify the functionality of individual methods or functions. Unit tests can be automated largely.
- Integration tests. Integration tests (unit integration) ensure that the components work as expected together. This involves the integration of units, classes, and components with other services. Integration tests can be automated largely and are highly usable for CI.
- Acceptance tests. Acceptance tests focus on business features and scenarios.
- UI tests. UI tests ensure that the application functions as expected from an end user perspective.

CI environment

**A CI/CD environment is similar to that of a production environment in which ongoing automation, monitoring, testing, deployment, and delivery takes place**. CI aims to reduce code integration and merging issues. The objective of the CI environment is to avoid integration challenges and keep code ready for the production environment with support from test automation. In a CI/CD and DevOps/CD environment using an Agile approach, development and operations collaborate closely together. The code changes are moved through a CI/CD pipeline designed to continuously integrate and deploy new product fixes, updates, and features. In the past, CI has used a separate tool for code build, monitoring, deployment, etc. However, many of the latest CI solutions on the cloud provide a fully integrated CI/CD solution.

The key benefits of CI are:

- It has a great focus on test automation to validate and ensure the product is not broken whenever new codes are integrated into the main repository. This saves time by identifying and addressing conflicts early on. This also helps develop a good automated regression suite for the software.
- CI helps to refine the code base through continuous integration and testing. CI also helps achieve high code coverage.
- CI reduces the scope of late integration defects and helps to identify conflicts early in the product development life cycle.
- The role of manual testing is reduced in CI. This helps QA engineers to allocate more time for debugging and tool support.
- CI reduces risk to software deployments as the releases are proved time after time on the CI server prior to production deployment. CI ensures the product is ready to be released at any time, so it is on demand and there are nearly zero downtime deployments.
- CI allows software products to reach the market much faster. The traditional phased software delivery lifecycle takes weeks or even months for a fully developed code to be in the market. CI helps the team work together, automate the build, carry out automated testing and risk-free deployment and ensure speedy environment provisioning.
- CI improves quality as the automated tools help to achieve quick regression testing. This helps the team find more time and effort for other testing activities, such as exploratory testing, usability testing, performance testing and security testing.
- Metrics generated from automated testing and CI (e.g. code coverage, code complexity and defect trends) help the team to improve overall quality.

CD involves packaging the software for deployment in a production-like environment. The primary objective of CD is to ensure that the software is always ready to go to production. The organisations that adopt CD can release numerous releases into production frequently, subject to passing all automated tests, and provide good test coverage. CD also enables roll back changes to take place quickly if something goes wrong.

2.2 TEST AUTOMATION AND BUSINESS MODELS

Software testing and test automation is planned and managed differently in different IT and business models such as IT consulting, SIs, MS/MV and MTS. In this section, we will address test automation in different business models.

2.2.1 IT consulting

**Information technology, consulting firms and consultants advise on the planning, design and implementation of information technology systems for their clients**. IT consulting focuses on advising organisations how best to use information technology in achieving their business objectives. IT consultants need strong interpersonal, technical, business and communication skills to deal with clients. IT consulting services are advisory services that help clients assess different technology strategies. Most consulting firms specialise in the advisory role, although many of them are supported by their system integration units to implement solutions. The well-known IT consulting firms, such as IBM, Accenture, Deloitte and Capgemini, have strong IT consulting arms along with system implementation expertise.

Testing and test automation are core parts of IT consulting. Some of the IT consulting firms offer **testing as a service (TaaS)** or testing consulting services from the advisory role to implementation. This section addresses how consulting firms support the client test automation process. Test consulting firms have a pool of test automation skills, and most of them offer this as a service. Experienced automation consultants from these firms bring expertise in various areas of automation such as feasibility studies, calculating ROI, managing test automation, implementing automation, independent testing, managing other **test automation service** providers and filling the skills gap.

Test automation and IT consulting characteristics:

- Identifying the right TAS – IT consulting companies have tremendous experience and expertise in various tools, tool implementation, automation strategies and frameworks generally used in a similar environment. This helps to avoid reinventing an automation solution from scratch and reduces the risk of failures in test automation.
- Tool procurement – Most IT consulting firms are partnered with tool vendors. This helps them to procure the tool quickly and cheaply. The tool procurement can be managed by the IT consulting companies with an additional marginal cost.
- Identifying and vetting the right external test automation partner – This involves identifying similar automation solution partners, assessing them and prioritising on behalf of the customer.
- Sourcing expertise in automated testing – This involves providing professional testing services’ resources from within the IT consulting company or externally.
- Advising on various testing services such as on-premises, cloud, TaaS and hybrid – This is mainly from IT consulting companies’ vast experience in test automation with different clients on different platforms.
- Building the automation framework – IT consulting companies have considerable expertise in this area and often reuse the expertise, components and framework from previous projects.
- Performing a test automation maturity assessment – IT and testing consulting companies have vast expertise in this area and have standard templates to perform test automation maturity assessments. They often have certified resources to assess test automation maturity.
- Implementing test automation processes and procedures – IT consulting companies generally have a pool of resources they can augment to deliver the test automation need for the customers.
- Advising on infrastructure for test automation – Many IT consulting companies perform an advisory and solution provider role for infrastructure for test automation and TASs based on IaaS, platform as a service (PaaS) and SaaS.

Limitations of test automation in IT consulting:

- Limited knowledge of client’s business operating model and infrastructure landscape – IT consulting companies and resources have sometimes limited knowledge of the client’s business and needs. It is difficult to build knowledge of the customer’s business quickly. They often tend to provide a standard TAS to the customer rather than a custom-made solution.
- The stakes on automation success and ROIs are often highly inflated – IT and test consulting companies tend to move to a ‘sale’ mode (sell the service) rather than focusing on a successful TAS. The solution is intertwined with the upselling objective.
- Test automation consultants are expensive – IT or testing consulting is often expensive as there is a premium charged on their reputation and expertise.

2.2.2 System integrator

A system integrator is generally an IT company that specialises in bringing together component subsystems into a whole with a group of similar providers with different skills. They deliver testing and test automation as part of the solution. System integrators primarily operate on two financial models: namely, **fixed time and fixed price (FT/FP)** or **time and materials (T&M)**. In fixed price, they often agree upon the scope of the work, the timeframe to deliver and the cost with the customer up front, with changes managed through change control. The time and materials model is generally used when the scope is not clear, and it is difficult to size the work.

Test automation works slightly different in T&M and FT/FP. In an FT/FP, the SI has a good amount of knowledge of the scope of testing, test automation, tools to be used, amount of work, test automation framework, timeframe and ROI. They mostly support both the solution development and post-go-live releases and continue maintaining the automated solution for the BAU phase. The fixed-price project generally includes the delivery of the first release of the system, and the test automation could even be omitted to reduce the cost. However, the test automation framework could be designed with the view to stay long term to support BAU activities if the SI is responsible for post-live maintenance of the solution. Most of the T&M models are approached with a different view as the test automation tools and tasks are not defined up front. Test SMEs use the T&M model to mitigate the unknowns of test automation.

Test automation and system integrator characteristics:

- System integrators have good knowledge of test automation. They have huge experience in delivering multiple systems across a variety of clients. SIs have expertise in end-to-end test automation, including functional and non-functional test automation.
- SIs have an existing partnership with major tool vendors and providers (such as Gold or Platinum partnership). They have the ability to procure tools on behalf of the customer at a reduced cost.
- They have a large pool of skill sets available within the organisation and prior experience in producing quick TASs and estimating ROIs.
- SIs have wide experience in automation solutions, tools and infrastructure. They have experience in defining test automation responsibilities.
- SIs have experience in the selection of the appropriate tool and automation approach and expertise in estimating the cost and benefit of tool usage. SIs also have the skills in training people to use the automation tools.

Limitations of test automation in system integrators:

- Lack of innovation and mainly template-driven (cookie-cutter model). SIs try to implement the same solution in all places to reduce the cost.
- Partner with a close network of vendors and tend to sell their products with a margin.

2.2.3 Multi-supplier and multi-vendor

An MS and MV model is where the client uses different products and solutions across a multitude of suppliers and companies on the same platform in order to develop a bespoke solution for a specific business need. The overall solution is managed and maintained by the customer, and they procure sub-solutions from different vendors. MS/MV requires more effort as there are a lot of different providers, solutions, platforms and infrastructure components on the same landscape. It is challenging to coordinate activities as some of these suppliers can be large consulting companies, IT service providers and product vendors. A single provider creates a dependency on one supplier and leads to high cost and opportunity loss; therefore, MS/MV avoids using solutions from a single vendor. A few major challenges in an MS/MV environment are:

- The customer’s IT organisation should be strong and mature enough to manage multiple suppliers.
- Unhealthy competition between solution providers.
- Risk of small vendor business closure or insolvency.

Test automation principles in MS/MV are very similar to those of the system integrator, enabling the customer to procure the optimal automation solution for their testing.

Test automation and MS/MV characteristics:

- Tool procurement and maintenance is the customer’s responsibility. However, the customer has a wide choice of automation tools and automation offerings from the suppliers.
- Suppliers can procure tools with less cost on behalf of the customer as they have a long-term relationship with tool vendors.
- Access to different service models, such as TaaS and MTS, is available for the customers through the MS/MV. This provides easily scalable and multiple test automation options. A pay-as-you-go TAS is also available for the customer through the MS/MV.
- Test resource augmentation through the suppliers is possible in MS/MV and this helps by requiring less time in setting up a test automation suite.
- Suppliers are experienced in similar solutions for other customers and reusability of the solutions is highly possible.
- Technical know-how and experience with previously used templates and solutions is available through MS/MV.

Limitations of test automation in MS/MV models:

- Large MS/MV environments are cumbersome, and generally lack support from other suppliers to automate the testing.
- Competition between suppliers is not always good.
- Suppliers are at times reluctant to support automation if they do not have any stake or financial benefits.

2.2.4 Product-based test automation

Software products are applications, solutions or systems delivered to the customer with documentation that describes how to use them. A few examples of software products are:

- Application software, such as Microsoft Office and Symantec Endpoint Protection
- Operating systems, such as Windows, macOS and Linux
- Internet browsers, such as Chrome, Safari and Edge
- Mobile applications, such as Instagram, WhatsApp and Skype
- Large enterprise applications, such as **enterprise resource planning (ERP)**, AWS and Microsoft Azure
- Games for all platforms, such as Roblox and Minecraft

The products are mainly created for multiple customers, and some products are customised for specific needs. Most of the software products are managed through the licence agreement, whether paid or unpaid. Product testing is different from the models discussed above in this chapter, as it involves some specific testing such as installation testing, patch release testing, localisation (L10N) testing and so on. Test automation has a major role in the success of the product, and ROI is high in product-based automated testing. Test automation adds huge value to product development and support.

Test automation is widely used in the product development environment. The products are generally tested on different platforms, and manual testing is cumbersome. The automated scripts can be used for different platform combinations, versions and patches. Security patches and the latest releases should be verified on different platforms. Regression testing is not possible without automated scripts.

Test automation and product characteristics:

- Test automation helps in achieving test coverage quickly on different platforms and environments.
- Test automation enhances repetitive, release and regression testing of regular upgrades, patches and hotfixes.
- Test automation enables a large user volume, and the stress testing required in product testing.
- Automated scripts can be used for many versions or releases in product testing.
- Installation testing can be quickly validated by test automation.

Limitations of test automation in product development:

- Continuous test suite maintenance requires product testing, and this involves additional effort and cost.
- High maintenance of the test automation suite is required due to additional requirements in upgrades, patch releases, multiple platforms and environments.
- It is less effective over a period as bugs may become immune to the automation suite.

2.2.5 Managed testing services

MTS cover all activities in a test project, including the entire testing process. Most of the IT offshore testing providers offer different flavours of MTS. Test automation is a key part of MTS. MTS and TaaS are used to represent the same concept, as both models grant on-demand access, ready to use testing services, high-quality consultants and proven solutions.

The below figure lists the common services offered by MTS models.

Figure 2.10 MTS pillars

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-10.png)

Note: SLA: service level agreement

‘Managed Testing Service is an end-to-end, fully customised service in which we take responsibility for test activities at either enterprise or programme level. A collaborative approach to sourcing testing and QA services, MTS is the solution for clients who want to transform their testing function and achieve high-quality systems cost-effectively, without the expense of large overheads and day-to-day responsibilities’ (Capgemini, 2014).

Test automation and MTS characteristics:

- Test automation is fully managed by the MTS provider and test automation can be predefined and pre-agreed in MTS.
- Test automation is managed and performed onsite, offsite and offshore, helping to save significant cost.
- High efficiencies, particularly in test automation and performance testing, and reduced deployment time.
- MTS offers fully managed test service and resource availability.
- Frees up in-house staff, enabling a focus on core business challenges and objectives.
- MTS offers training as a service.
- A shift from capital expenditure to usage based on operating expense.
- Total flexibility to use as needed (subject to the price), reducing fixed testing overheads.
- Access to increased test automation capacity.
- MTS can provide advanced test environments and access to the latest tools, devices and platforms for test automation.
- Measurable quality improvements in the MTS model.

Limitations of test automation in MTS:

- Constant liaison with the business for decision making, and a high dependency on in-house resources, for example data for test automation
- Loss of in-house skills and expertise in test automation
- Hidden costs such as additional tool features and test automation dashboards
- Numerous change requests for enhancing test automation scope and additional features

2.2.6 Start-ups, small and medium enterprises

Start-ups are generally new companies founded by one or a few aspirational individuals to create a unique product or service. They are in the initial stages of business and so mostly face the challenge of getting off the ground while simultaneously trying to attract investment. There is a high expectation for start-ups to get their products or services in the market with limited resources. Therefore, in most start-up organisations the employees tend to stretch their roles to various areas beyond their titles. A similar establishment is small/medium scale businesses, which are enterprises or corporations which generally operate with a low initial investment or have a small number of employees.

Start-ups and small/medium sized businesses often try to optimise resources. They have similar characteristics, such as limited hiring experience, lack of an established HR department, established company reputation, limited resources, new IT department, new tooling team and so on. However, in general the whole team is passionate about the business and want it to succeed.

Most of the small or medium business houses are driven by market demands and so are the first to market. They often lack IT tools, processes, and documentation, for example a small sized company may use a spreadsheet or a free open source tool for defect management compared to a licensed and procured popular test management tool. They often focus on immediate needs, such as quickly fixing the defect and moving onto the next one rather than gathering test metrics. Reusability is a key ethos in start-up and small/medium sized organisations, where test automation plays a key role. They tend to reuse the existing solutions available in the market with minimum rework. Software is often developed and tested with agility. They often avoid detailed planning, documentation, and developing an automation framework, and instead start to automate and deliver the working solution on day one. Testing is important for start-ups that focus on ‘technology first’ where the business depends on having an application or solution that delivers what it is selling.

Documentation is a core part of any IT project. The level of documentation varies across projects, programmes, products, companies, and industries. In start-ups and small/medium sized organisations, the documentation is often a few lines in an email or a wiki page rather than a detailed ‘change controlled’ process. The documentation is important in testing and test automation. However, it should be realistic and fit for purpose. Start-ups and small/medium sized organisations tend to focus on a ‘what is fit for purpose’ or ‘immediate objectives’ approach during their documentation process.

The characteristics of test automation in start-ups and small/medium organisations are as follows:

- Agile-based development, testing, and test automation is often practiced. The focus is on immediate goals.
- Software testing and test automation is vital at every stage of development. CI, Lean, Kanban and DevOps are often practiced.
- Products are developed based on MVP, which is generally followed to get a sense of user engagement.
- Reusability of testing strategies and test automation is crucial as it reduces cost and helps in delivering the solution quickly.
- Testing and test automation are important as they have very little space for error.
- Free and open-source software are very popular due to low cost and ease of setting up.

Limitations of test automation in start-ups and small/medium organisations are as follows:

- Limited budget and time to test the solution on every possible permutation, combinations, configuration of devices and environments.
- Less focus on quality in the process and documentation.
- Testing and test automations are often side-lined due to focussing on delivering a working solution.

2.3 TEST AUTOMATION IN FUNCTIONAL AND NON-FUNCTIONAL TESTING

Functional testing validates the expected features of a solution, and non-functional testing validates the scalability and sustainability of the solution. Both are success factors for any solution and supported by automated testing.

2.3.1 Functional testing

Functional testing validates the solution against functional requirements and specifications. The purpose of functional testing is to verify that the solution works as expected in line with requirements. The key types of functional testing are:

- Unit testing
- Unit integration testing
- Smoke testing
- System testing
- Integration testing
- Regression testing
- Exploratory testing
- User acceptance testing

The functional requirements for a solution are generally described through the products shown in the below table.

Table 2.3 Functional requirements specifications

|                                                          |                                                                                               |
| -------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Product                                                  | Description                                                                                   |
| User stories and epics or business requirements document | Statement of high-level functional requirements                                               |
| Requirements specification                               | Statement of functional requirements                                                          |
| Interface definition documents                           | Detailed interface specification(s) for each interface                                        |
| Wireframes                                               | Page designs                                                                                  |
| User experience design                                   | Look and feel page designs based on wireframes                                                |
| Product backlog                                          | Comprehensive list of requirements used to drive the detailed design and development activity |

The below figure shows the key areas of test automation in functional testing.

2.3.2 Non-functional testing

Non-functional testing is validating the solution for its non-functional requirements, the way a system operates, scalability, sustainability and other software quality characteristics. Functional and non-functional tests, testing types and stages are often used interchangeably because of the overlap in scope between requirements. For example, security testing is often used for security accreditation validation, penetration testing and vulnerability scanning, and performance testing is a broad term that includes many specific requirements such as load, soak, volume, response time, capacity, reliability and scalability. A functional test, for example, is to check a report is working as expected, displaying the correct data as per the calculations, and a non-functional test is to check that the report loads within a defined time, for example 5 seconds. The key types of non-functional testing are:

Figure 2.11 Functional test automation types

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-11.png)

- Usability testing
- Performance testing
- Load/volume testing
- Scalability testing
- Availability testing
- Supportability testing
- Maintainability testing
- Security testing
- Regulatory and legal testing, for example accessibility testing
- Compliance, standards and policies testing
- Access testing, for example single sign on (SSO)
- Compatibility testing
- L10N and internationalisation (I18N) testing

The non-functional requirements for a solution are generally described through the products shown in the below table.

Table 2.4 Non-functional requirements specifications

|                                                           |                                                                            |
| --------------------------------------------------------- | -------------------------------------------------------------------------- |
| Product                                                   | Description                                                                |
| User stories and epics or business requirements document. | Statement of non-functional requirements.                                  |
| System architecture or high-level design.                 | Architecture views of the solution, including non-functional requirements. |
| Interface definition documents.                           | Detailed interface specification(s) for each interface.                    |
| Component design architecture or low-level design.        | Detailed architecture for each component.                                  |

The below figure shows the key areas of test automation in non-functional testing.

Figure 2.12 Non-functional test automation types

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig2-12.png)

2.3.3 Testing stages

The following testing stages and types are performed generally as part of the solution development. The functional and non-functional tests, testing types and testing stages are often used interchangeably because of the overlap in scope between requirements.

- Unit testing/component testing (UT/CT) and component integration testing (CIT)
- System testing (ST)
- Factory acceptance testing (FAT)
- System integration testing (SIT)
- User acceptance testing (UAT)
- Performance and volume testing (PVT)
- Operational acceptance testing (OAT)

The below table describes the test stages, types and respective test automation.

Table 2.5 Testing stages and automation

|                                                                     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                                                                                                                    |
| ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Test stage                                                          | Key objectives                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Test automation                                                                                                                                                                                                                                                                                                                                                    |
| Unit testing or component testing and component integration testing | To prove that each developed software component (or package configuration) functions according to its technical specification and that deployed unit components interoperate as expected.                                                                                                                                                                                                                                                                                     | Unit testing and unit integration testing are largely automated. There are various tools and packages available to automate unit testing. A unit test can be 100% automated and provide high returns. A few widely used unit testing tools are JUnit, [xUnit.net](http://xunit.net/), NUnit, TestNG, PHPUnit, Symfony Lime, Test Unit and RSpec.                   |
| System testing                                                      | To test that the solution or system meets the specified functional and non-functional requirements for different types of valid or invalid conditions.                                                                                                                                                                                                                                                                                                                        | System testing is highly automated for both functional and non-functional requirements. There are many tools and frameworks available to automate both functional and non-functional requirements such as UFT, Selenium, Tosca and Eggplant.                                                                                                                       |
| Factory acceptance testing                                          | To ensure that the solution is fit for deployment into the customer’s environment for full-release testing.                                                                                                                                                                                                                                                                                                                                                                   | FAT is subject to the business domain and how different each installation is. Optimally, all automated tests can be executed to validate the installation (site or factory).                                                                                                                                                                                       |
| Systems integration testing                                         | To ensure that the solution integrates and functions in end-to-end internal and external systems with no data loss or corruption.                                                                                                                                                                                                                                                                                                                                             | This is similar to system testing and highly automated for both functional and non-functional requirements. There are many tools available to automate both functional and non-functional requirements.                                                                                                                                                            |
| User acceptance testing                                             | To verify that the solution is fit for purpose from a business perspective, i.e. business requirements and user acceptance criteria have been met. This is usually performed by the end-users or business users, or their representatives.                                                                                                                                                                                                                                    | UAT generally follows manual testing. However, payment, security, data migration and parallel process testing are usually automated as it is not feasible to test them manually. In Agile, a large part of UAT tests are automated as acceptance test-driven development (ATDD) and behaviour-driven development (BDD) are derived from the epics or user stories. |
| Performance and volume testing                                      | To verify that the solution meets the specified performance requirements when placed under different levels of load, e.g. under normal, peak and extreme workloads. Load variations may include the number of users, the volume of transactions and the volume of data.                                                                                                                                                                                                       | Most performance tests require functional or performance testing tools to run effectively. Some commonly used performance testing tools are:<br><br>- LoadRunner<br>- JMeter<br>- Silk Performer                                                                                                                                                                   |
| Operational acceptance testing                                      | To provide operations and support staff with confidence that the system operates correctly in the production environment and can be managed by them. Tests typically focus on support readiness, testing issue resolution through the service desk, and operational support aspects like backup, archiving, monitoring or alerting, recovery point objective (RPO), recovery time objective (RTO), maintenance, disaster recovery, scalability, reliability and availability. | OAT is performed using a mix of manual and automated testing. Backup, archiving, monitoring, alerting etc. are widely automated using various tools. However, disaster recovery, failover etc. are generally performed manually.                                                                                                                                   |

2.3.4 Testing types

According to the International Software Testing Qualifications Board (ISTQB) definition, testing types are a means of clearly defining the objective of a certain level for a programme or project. The tester focuses on a particular test objective during test case execution. The below table describes the different types of testing and the role of test automation.

Table 2.6 Testing types and automation

|                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Test type                             | Objectives                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Test automation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Static testing and static code review | Analysis and review of test base material (e.g. functional requirements, non-functional requirements, high-level design (HLD), low-level design (LLD), full system architecture, detailed design architecture) to verify that the building block specifications of the solution are unambiguous and provide sufficient information.                                                                                                                                                                                                                                                                                                                                                                                                                                                          | This is largely manual testing; however, test management and version management tools bring discipline to this activity. An automated review comment tracker ensures comments are addressed quickly and reduces manual effort. Tools such as Microsoft SharePoint, Microsoft Azure DevOps or Micro Focus Application Lifecycle Management can be used for review comments tracking. Static code reviews are supported by tools like Git or Bamboo.                                                                                         |
| Functional tests                      | To test that the delivered functionality within the application meets the specified requirements.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Functional tests are largely automated subject to the ROI, benefits and qualification of the right test automation candidates. Some common tools used for automated functional testing are:<br><br>- UFT<br>- Tosca<br>- Selenium<br>- Eggplant<br>- Appium                                                                                                                                                                                                                                                                                |
| Regression tests                      | To test that the application has not been negatively impacted by the introduction of new functionality, changes or fixes, i.e. tests to verify that what was working before still works.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Same as functional testing, regression tests are largely automated subject to the ROI, benefits and qualification of the right test automation candidates. The same tools for functional test automation are used for automating regression testing.                                                                                                                                                                                                                                                                                       |
| Business cycle tests                  | To emulate the activities performed by the application over time periods such as daily, weekly or monthly and ensure that the application performs as specified end-to-end.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Test automation adds high value to business cycle tests such as periodic reports, payroll and parallel processing. There are specific tools available for business cycle test automation alongside functional automation tools. Microsoft Excel with macros is very useful in this testing.                                                                                                                                                                                                                                                |
| Data migration testing (DMT)          | DMT is also known as extract, transform, load (ETL) testing. This is to verify that the data routines specified are operating correctly and that extracted data can be loaded onto the new platform with no loss of integrity of data. This tests that the data load and migration processes function properly.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Data migration is certainly a candidate for 100% automation. Manual data testing is prone to error and not feasible for large migrations. This is largely automated testing. The widely used data migration testing tools are: QuerySurge, RightData, BiG EVAL, iCEDQ and Informatica Data Validation.                                                                                                                                                                                                                                     |
| Load testing                          | Testing of the system’s performance for designated transactions or business functions under different workload conditions and across different time periods.The following should be reflected in the performance testing:<br><br>- Response times (interactive work) for end-users, defined by averages or percentiles<br>- Processing times (scheduled activities), defined by averages or percentile<br>- System throughput – The amount of data passing through a component or system in a given time period or the amount of work performed by a computer within a given time<br>- Concurrency number of users working with and idle while being logged in the application at the same time<br>- Scalability – The ability to be enlarged to accommodate growing amounts of work or data | Mostly automated unless the number of users is minimal. There are various tools available for load testing.                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Endurance (soak) testing              | To verify that the application can sustain continuous expected loads without performance degradation.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Same as for load testing.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Failover testing                      | To verify that the system can successfully failover and recover from a variety of hardware, software or network malfunctions without undue loss of user interface, data or data integrity.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | This is largely manual testing and coordinated between many other non-functional aspects such as event management, monitoring and alerting.                                                                                                                                                                                                                                                                                                                                                                                                |
| Resilience testing                    | To test the ease with which the application handles and recovers from failure scenarios such as power failures, communication failures and software component failure.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | This is generally performed manually. However, this can be partially automated. The load testing tools can be used in resilience testing, and AI-generated testing can be used to automate resilience testing.                                                                                                                                                                                                                                                                                                                             |
| Accessibility testing                 | To test that the application or web content is accessible to people with disabilities. It is about building digital content and applications that can be used by a wide range of people, including those with visual, auditory, speech or cognitive disabilities.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Accessibility testing is performed as a combination of manual and automated testing.The following tools are commonly used for accessibility testing:<br><br>- Dragon Naturally Speaking<br>- Dolphin SuperNova Magnifier and Screen Reader<br>- ZoomText Magnifier/Reader<br>- Job Access With Speech (JAWS)<br>- Read and Write Gold<br>- ClaroView<br>- OpenDyslexic font set                                                                                                                                                            |
| Security tests                        | To test that the application meets specified security objectives.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Security testing is mostly automated using specific tools and hardware. Product-based companies maintain an in-house security test team to conduct testing. However, customers use external suppliers to perform penetration testing in an SI and multi-supplier environment to ensure that the testing is independent.                                                                                                                                                                                                                    |
| Penetration (pen) testing             | Pen testing is a type of non-functional testing (white box or black box) that is done to check whether the IT solution is secured or not. Usually, it is an authorised simulated attack on a system that looks for security weaknesses, potentially gaining access to the system’s features and data. Pen testing is to verify that the solution meets specified security objectives. This testing may be carried out by a third party.                                                                                                                                                                                                                                                                                                                                                      | This is largely automated and performed independently. Some areas of testing can be performed manually, such as user access testing or quality scans. Development teams generally perform manual security testing and vulnerability scanning. A combination of manual testing and automatic security scans reduces potential vulnerabilities, along with penetration testing. Security testing is performed at the end of the development process on the final version of the code that will be implemented into a production environment. |
| Compatibility testing                 | To test that the application functions correctly under varying permitted configurations, e.g. different web browsers or user device types.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Compatibility testing is performed as a combination of manual and automated testing using specific tools. The most common areas for compatibility are browsers, operating systems, desktops, mobiles, tablets and mobile networks.                                                                                                                                                                                                                                                                                                         |
| Installation testing                  | To test that the application can be installed, both as a new application and as a new release, and that it then operates correctly.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | This is largely automated testing.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

2.4 TRENDS

A trend is a general direction in which something is changing or developing, and in test automation, there are visible trends in increasing demand for tools based on AI, ML and deep learning (DL). In this section, the current trends in test automation tools are covered.

2.4.1 Artificial intelligence, machine learning and deep learning

AI and ML are two upwardly trending fields in recent years, and AI will soon be a tester’s best friend, according to the World Quality Report 20–21 (Capgemini, 2020). Artificial intelligence enables a machine to simulate human behaviour, and machine learning allows machines to learn from past data without explicit programming. AI and ML are not the same things. At a high level, AI uses ML for knowledge and learning to form intelligent behaviour. AI, ML and DL enable machines to learn, adapt, take decisions and execute through their experience. The intelligence supported by algorithms helps machines to influence the decision-making process and improve over time. Machine learning uses DL for large data management and is about processing large data sets. The DL designs are inspired by human neurons. DL is an AI function that mimics the workings of the human brain in processing data and creating patterns for use in decision making. Many codeless test automation tools use AI to learn from humans, triaging script failures to make tests less flaky.

AI in software development is evolving rapidly, such as in self-driving systems and voice-assisted control. AI-based test automation tools make the testing life cycle easier. There are many testing tools that use an AI-based framework for testing. The AI reduces the direct involvement of the developer or tester in testing. The AI-enabled testing tool reviews the current test status, recent code changes, code coverage and other metrics to decide the test approach, what should be tested and when. This reduces the overall testing effort.

2.4.2 Robotic process automation

RPA is a business automation technology that automates routine, repetitive tasks without human intervention. RPA uses software bots (robots) that interact with the system like humans. RPA is heavily used to automate business processes that are rules-based, structured and repetitive, for example most of the online credit card application processing and personal loan application processing uses RPA to analyse the data, perform a credit check and automatically approve or reject without any human intervention. An RPA ‘robot’ is a piece of intelligent software to handle repetitive, rule-based digital tasks. A good example of an RPA bot is an internet search engine spider that crawls websites to update search engine indexes. Financial firms were the early adopters of RPA, but there are now companies in many industries, including healthcare, retail and manufacturing, that use RPA technology. RPA systems develop the action list based on end-user interactions on the application’s GUI and then perform the automation by repeating those tasks directly in the GUI.

Robotic process automation is a business automation technology that automates routine, repetitive tasks without human intervention.

There are many tools used for process improvement and these tools fall into two buckets: those that help to investigate and trial possible process improvements, and those that apply the improvement. Process mining tools assist a business process owner to investigate possible process improvements, and RPA/AI tools automate the process. RPA is business process automation and is not business process management. RPA does not provide an end-to-end solution for business management. It uses AI, ML and inputs from multiple sources to make decisions, and it does not process non-electronic and unstructured inputs. RPA provides impressive results for business process automation and offers tremendous value. However, there are many RPA implementation failures. It is common to underestimate the cost and time to implement RPA solutions. RPA provides a tool for testers and business users performing testing, especially in implementing large-scale standard systems like SAP, Oracle and Salesforce.

RPA itself is an automation process. Testing is a component in the RPA life cycle as it needs to be tested and certified that it works as expected. RPA tools are not test automation tools like Selenium or Unified Functional Testing (UFT). For example, Selenium automates the testing of web applications, and RPA automates business processes. Tools such as UiPath, Automation Anywhere and Blue Prism are used for RPA automation.

Many test automation tools are used for RPA automation, for example Selenium scripts can be used for a web-based SUT and can run as RPA in the production environment. However, there are many tools specifically designed for RPA that provide specific features for RPA.

The RPA life cycle involves the following main steps:

- Analysis
- Bot development
- Testing
- Maintenance

RPA requires end-to-end testing to ensure that it works as expected. Generic tools such as UFT and Tosca can be used for RPA automation. ‘Record and play’ is a suitable and quick solution for RPA test automation. RPA tools are also used in test automation, allowing for codeless automation; they can also be used for regression testing.

The main benefits are:

- Quick regression test pack creation
- Easy scalability
- Business process validation
- Real-time visibility of testing and test progress
- Test on the production environment

To summarise, test automation is a process of automating the testing procedures using a code or software tool such as Selenium or UFT, and RPA is a practice of automating the business process using software robots.

2.5 SUMMARY

In this chapter, we addressed test automation in a variety of IT business models, development processes, and different types and stages of testing. There are a variety of factors to be considered in the decision-making process, as the success of the test automation is dependent on the influencing factors more than the automation tools. The first two chapters will help you to decide if test automation is a viable option to support your overall testing needs. In the next chapter, we will help you choose the right tool for automated testing.
