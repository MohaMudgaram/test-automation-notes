## ENVIRONMENTS

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

Environments play an essential role in the success of test automation. This chapter covers various IT infrastructure and environments and their role in automated testing.

The test automation framework and automated test suites are designed to work independently of environments. An environment-specific automated test suite will limit the opportunity to reuse the automation suite.

A test environment is a collection of software and hardware in which the testing takes place, and is generally a cut-down version of a production environment. An integrated test environment is a ‘federated’ environment that is representative of the end-to-end solution to prove that the proposed solutions work together.

Test automation needs to verify the test environment is working as expected. An ideal automation test suite will be independent of environments, platforms, browsers and mobile devices, that is, cross-platform compliance. Maintaining a separate automation suite for different environments is not feasible and is effort-intensive. Most test automation tools offer cross-platform compliance.

A large US-based product development company used automated testing for release and regression testing. The company has the same product lines in different platforms such as Windows, macOS, Linux, IRIX and Unix, along with multiple browsers and mobile versions.

The products often go through changes, patch updates and hotfixes. Regression and release testing were a challenge to perform on all the platforms and devices.

After a detailed study, the test automation team developed a custom framework to support cross-platform testing. The automated testing followed a data-driven automation suite for release and regression testing. A spreadsheet was used to manage cross-platform testing, a simple data sheet that listed all the different platforms and versions with scope and out-of-scope sections. Based on the scope value the automation suite included a selected platform for testing.

The automation team anticipated cross-platform requirements and developed libraries to manage to test for all different versions and platforms. The test execution was managed from a simple spreadsheet with ‘yes’ or ‘no’ values.

6.1 TEST AUTOMATION ENVIRONMENTS

The technical and security specifications of different environments are a challenge when designing and developing the automation suite. The test automation approach should be designed in line with the DevOps or cutover and release approach of the solution to ensure that the test automation suite and the automation framework function independently in different environments. Test automation is expected to work on various environments and infrastructures with minimum changes.

A test environment is a set of software, devices and infrastructure in which the testing team tests the SUT.

The major environments are:

- Development
- Test
- Production support
- Production

Each of these environments may consist of multiple sub-environments, such as system testing, system integration testing, end-to-end integration testing and performance testing. Building and managing test environments efficiently and effectively in line with the test automation strategy helps to achieve successful test automation outcomes. This can deliver significant benefits and substantial cost savings for the organisation.

The below table shows different environments and their features.

A key principle in the provision of the automation test environments is that they should closely resemble the architecture, configuration and release process of the target live or production environment, for example if the live environment is hosted on physical servers (e.g. on premises) then testing using environments hosted on virtual servers (e.g. cloud) can introduce additional risk.

6.1.1 Development

The development environment is where development takes place. This can vary from a developer’s desktop to a fully configured and version-controlled system. A development environment is a place where most of the unit test automation preparation takes place. This environment is hosted within the internal network, and not all infrastructure or platform releases may be applied.

Figure 6.1 Test environment sequential diagram

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig6-1.png)

Table 6.1 Environments and their features

|                                     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Environment                         | Features                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Development                         | Product development is conducted in the development environment.Used for automation test preparation.Generally, conducted outside any configuration management processes to allow for a ‘DevOps’-like delivery approach.Used for compiling build and proving release items.Emulation models and test stubs used for inbound and outbound components.Development or infrastructure team is responsible for this environment.                                                                                                          |
| Testing or staging                  | Testing takes place in the test environment.Automation test execution takes place in this environment.Release and deployment are configuration managed.Generally owned by the testing team.Automated regression suite is used in this environment to prove the build stability.Emulation models and test stubs are used for inbound and outbound components as required.                                                                                                                                                             |
| Pre-production or business as usual | The pre-production environment is generally an informal environment used to verify the connectivity with existing infrastructure and applications.The pre-production environment is generally a fully integrated environment to prove the end-to-end connectivity between source and target systems.This environment is generally used for performance testing and early application security testing.The pre-production environment is generally used for UAT and live support.Automated test suite is used for regression testing. |
| Training                            | The training environment is a ‘nice to have’ environment to allow UAT and training activities to be performed independent of each other.This environment is owned by the business or the product team.                                                                                                                                                                                                                                                                                                                               |
| Production/live                     | Release and deployments are configuration managed.Jointly owned by the IT, business and product teams.                                                                                                                                                                                                                                                                                                                                                                                                                               |

The benefits of using the development environment for test automation are:

- Early automation is possible as it is the first environment in line.
- Test automation can start along with the development.
- Test automation can be used to build validation and smoke testing.

The challenges of using the development environment for test automation are:

- Unstable application and constant code and infrastructure changes. A stable SUT is recommended for automated functional and regression test preparation.
- The development environment is not a true representation of the production environment for automation.
- The automated test pack may require changes in other environments prior to execution.
- Stubs and drivers are generally used to develop the SUT and automated test scripts, and this may impact the quality of the automation test suite.
- Regular backup for the automation test scripts may not be possible.

6.1.2 Test

The test environments cater to the test team, allowing them to verify the solution functions according to the specified requirements. The test environment can be stand-alone or integrated. The integration test environment is used to test the inter-process communications to ensure that the system parts function together correctly. The cloud infrastructure provides the opportunity to spin off any environment quickly, in almost the same way as the production environment. Most cloud providers specify clear guidance for code development and release.

The common test environments are:

- System testing
- System integration testing
- End-to-end integration testing
- Non-functional testing

The test environment is the right place to commence test automation, as it is built for testing, configuration management and release control.

The benefits of using the test environment for test automation are:

- This is a dedicated environment for the testing and owned by the testing team.
- Test data from manual functional and regression testing can be used for automated testing.
- Support from the wider testing team is available for automation, for example functionality walkthrough and test data creation.
- Stable SUT avoids frequent changes to automation scripts.

The challenges of using the test environment for test automation are:

- The latest source code from the development environment may not be available.
- Test environments are not a true representation of production.
- Testing tool installation and configuration requires full access to the environment.
- Regular backup for the automation test scripts may not be possible.

6.1.3 Production support or pre-production

The production support or pre-production environment is generally a ‘live-like’ or sometimes a scaled-down version of the production environment. The purpose of this environment is to support the ‘live’ system. This is generally used as the final gate to deliver to the production environment. This environment is used for UAT in many places and supports the investigation of issues raised within the production environment. This is also used as an isolated platform for upgrades, patching, bespoke code and data releases, which are to be informally applied before being applied to production. This environment can also be used for usability and accessibility testing if required. This environment is a better representation of the target production environment and can be used to support the key non-functional test stages.

The benefits of using the pre-production environment for test automation are as follows:

- Pre-production and production environments are identical and are a true representation of production for automation.
- The pre-production environment helps to run test automation in an exactly production-like environment.
- The latest features are available for test automation, despite being not yet available in the production environment.
- Pre-production environment is widely used for automated performance testing.

The challenges of using the pre-production environment for test automation are the following:

- The latest source code from the development and test environments are not available for test automation.
- The pre-production environment is shared with other teams such as performance testing and UAT, and this can impact the stability of the environment.

6.1.4 Production

This environment will be used to deploy the final solution and may be used to support some of the non-functional test stages, such as penetration testing and security testing.

The benefits of using the production environment for test automation are as follows:

- Live features are available in the production environment.
- The SUT is already available to the end-users and customers, and so it is a true representation of the final solution.
- The production environment is widely used for product testing, for example beta trialling.
- Automated regression testing on the production environment provides a quick view of the SUTs.
- The production environment is widely used for automated security testing and disaster recovery testing.

The challenges of using the production environment for test automation are the following:

- Any testing in the production environment can impact the stability of the environment, and it can affect the end-users and the business.
- The solution is already live, and any defects identified in production take time to fix and roll-out.

6.2 SUMMARY

This chapter is an introduction to different environments and their roles in the success of test automation. It addressed some of the benefits and challenges of using different environments for successful test automation. Next, we will explore candidates for test automation.
