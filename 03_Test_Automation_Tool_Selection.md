## TEST AUTOMATION TOOL SELECTION

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

Introducing test automation to the IT landscape is a management decision, and previous chapters described various factors supporting this decision making. Once the organisation decides to go for automation, the next important activity is automation tool selection. Most widely and commercially used functional testing automation tools are based on object-oriented programming (OOP) or scripting languages. There are many custom-developed tools based on scripting languages such as JavaScript and Shell script. It is important that the tool selection should be in line with the skills available in the team. There are plenty of tools available for test automation, and it is important to select the right tool to automate the solution. The IT market is filled with automation tools, but not every tool suits the requirements and tool vendors tend to offer their tools as the best solution for automation.

This chapter will help you to understand the process of choosing the right automation tool. The first part of the chapter addresses the factors to be considered for tool selection and additional factors to be considered for tool assessment. The second part of this chapter addresses tool selection criteria. 

3.1 TEST AUTOMATION TOOL SELECTION

In this section, there is a list of factors to help you in deciding on an automation tool; the tool selection criteria are different for product, project, technology, organisation and project implementation methodologies. All these factors should be considered when selecting a tool for automation needs.

The following generic factors should also be considered:

- Usability of the tool or ease of use
- Functionality applicable
- SUT, infrastructure and tool compatibility
- Compatibility with other project tools, for example in a DevOps environment, the testing tool’s ability to be integrated with other development tools
- Maintainability and support of the tool
- Initial and ongoing cost
- Flexibility to adapt to changing requirements

A large retail company in North America reviewed a set of automated testing tools for its web application. The test team decided to use both manual and automated testing as part of the solution to validate the ecommerce application. The tool selection team considered different options fit for both desktop and mobile test automation. Following a detailed analysis of requirements and user distribution, the team selected a mobile automation tool since more than 80 per cent of traffic originated from mobile and tablet devices.

The following criteria should be considered when choosing an automation tool.

3.1.1 Requirements

Requirements are key factors influencing tool selection, and therefore a detailed review of the functional and non-functional requirements is essential before choosing the right tool. Obtaining a deep understanding of the automation requirements, such as solution type (e.g. web, desktop, mobile, on-premises, cloud, hybrid, DevOps, Waterfall, Agile), scope, how testing is to be conducted, post-live test support, percentage of automation, release frequency and the existing team’s strength in programming languages, is a key requirement for test automation and tool selection.

A large ERP implementation programme manager decided to procure a tool for its quarterly release regression testing. In the process of tool selection, one of the key requirements was to select an automation test tool to support quick regression testing of the quarterly patch release.

The team reviewed three tools:

1. An open-source tool
2. The tool currently used in the organisation
3. A third-party automation tool recommended by the ERP vendor

The team selected the third-party automation tool recommended by the ERP vendor, even though this tool had the highest annual licence fee, as this was the most suitable tool for their needs. Although the next option was a low-cost, effective tool, this tool required a minimum of 30 per cent changes to the automated test suite prior to the execution of every release. This was not a viable option for the programme.

The outcome of the tool selection process is expected to provide multiple options, including one with ‘No Automation’ and a ranking of the tool recommendations.

3.1.2 Organisation structure

The organisation structure is an important factor for tool selection, along with the cost and ROI model.

Product development companies have a clear understanding of their requirements for automation, with costs estimated up front and budgets allocated. The tool selection process considers the current products and application in scope and future product lines prior to selection. The technology, programming languages and requirements such as smoke test, regression tests, release cycle and trialling all influence the tool selection.

Organisations that are heavily dependent on external suppliers and have outsourced IT operations have a different approach, and cost management is the main parameter for tool selection. The tool is usually funded by the customer organisation, with third-party suppliers implementing the test automation on behalf of the customer. However, it is likely that the supplier may opt for a low-cost solution if the tool cost and implementation are included in the overall supplier cost. Organisation structure and IT operating models such as fixed price, time and materials, multi-supplier, multi-vendor, product-focused, IT consulting and system integrators influence the tool selection process. The customer organisation needs to set the expectation up front with the suppliers, to provide them with a list of target test automation tools and tool selection criteria. This will deter suppliers from selecting the cheapest test automation tool to reduce their cost over the most suitable tool for the customer organisation.

3.1.3 Development approach

Test automation goals and objectives must be aligned with the IT solution development approach to maximise the benefits. For example, in a DevOps environment, the test automation approach and tool selection need to be aligned with the Agile way of development and support DevOps delivery. The selected tool should be integrated into the solution and the development methodologies used for the implementation. The development schedule plays a major role in test automation tool selection.

3.1.4 Testing objectives

Testing objectives, such as quick regression testing, smoke testing, DevOps, functional automation to support Agile development, UAT coordination and interim patch release, are key influencing factors for appropriate automation tool selection. For example, if the testing objective is to provide a day one TAS to support the DevOps, most likely the team will choose a tool that can be procured easily and require minimum infrastructure to set up and to commence automated testing.

A large retail company in the UK decided to introduce test automation to support its multi-supplier environment. One key objective of the in-house test team was to manage the UAT with a geographically distributed team. After a detailed analysis, the test team selected a cloud-based test management tool to coordinate UAT test case execution and defect management for its globally distributed team. This tool provided a platform for test case execution, defect reporting, tracking, triaging and the management of all the acceptance testing in one place.

3.1.5 System environment and technology

Solution implementation environment and technology are critical factors for tool selection. In recent years many organisations have moved from on-premises to cloud and hybrid environments for solution development, infrastructure and test automation. Testing tool selection should be aligned to the environment and technologies to achieve the expected benefits. A tool that only supports cloud-based solutions may not be suitable for on-premises and hybrid solutions. On-premises requires tools to be downloaded and manually installed by physically or remotely accessing the environment. The infrastructure needs to be provisioned to support the operational aspects of the testing tool, such as access to the environment or periodic patch update. However, a cloud environment may allow an SaaS-based testing tool and periodic automatic patch releases. The testers may be onsite for test automation in a secure environment, and this can be an obstacle for a cloud-based tool supported by an offshore testing team. Testing tools require support from the vendor, known as professional services, and an on-premises client or server environment can incur additional costs over a web-based cloud solution.

3.1.6 Return on investment

ROI is a key factor for tool selection.

3.1.7 Automation costs

The cost of automation is another factor for tool selection. Some tools have low licence fees but may require high maintenance. A few indicators to identify costs are:

- Implementation effort.
- Licence fee and renewal fee.
- Annual maintenance fee.
- Hardware and hardware support cost.
- Infrastructure cost such as cloud service support fee.
- Hosting platform: cost involved to maintain the platform or the licence cost for the software on the platform.
- Professional services charged by the tool providers.
- Cross-functional support by other teams.
- Script maintenance and enhancement such as ongoing maintenance or enhancement of the script.
- Tool training cost.
- Architecture: the complexity of the system architecture is an indicator of how much effort and cost is likely required to be invested.

The below figure is a representation of the relative cost of the tools widely available in the market.

Figure 3.1 Automation tools versus cost matrix

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig3-1.png)

3.1.8 Proof of technology and proof of concept

PoT and PoC are two activities involved in tool selection. PoT is a small project that tests whether an idea about technology is viable, and PoC is a procedure that tests whether a tool fits by analysing it using various parameters. The objectives of PoT and PoC are to verify that the tool can work on different applications and is fit for the organisation’s automation needs. It covers the following activities:

- Tool comparison
- Reviewing sample test scripts covering various scenarios
- Automating a few sample scenarios
- Verifying the tool’s ability to manage data and support frameworks
- Ability to operate in the IT estate or infrastructure

The PoCs are generally supported by the tool vendors with an evaluation version of the tool.

PoT is a small project that tests whether an idea about technology is viable, and PoC is a procedure that tests a tool’s suitability by analysing it on various parameters.

3.2 TOOL SELECTION ASSESSMENT

After collating the list of requirements to be met by your TAS, the next step is to create a comparison matrix to do the tool selection assessment. There are various templates available to support the tool selection process. Tool selection criteria vary based on the organisations’ needs and requirements. See below figure for the workflow for tool selection.

Figure 3.2 Tool selection process

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig3-2.png)

The following factors should be considered when customising the template for your organisation’s tool selection assessment:

- Tool usability. Some test automation tools are difficult to learn and hard to use.
- Functions available such as automated reporting, recovery and backups. These features help in saving test automation effort.
- Compatibility with other project tools such as defect management tools and automated build validation. This is essential for DevOps.
- Maintainability such as scripts and frameworks.
- Support from either the vendor or the community.
- Initial and ongoing cost such as tool procurement, renewal, path updates or the cost for the add-on to enhance the features.
- Flexibility to adapt to changing project or product requirements.
- Training, documentation and tutorials available to support the tool and the test automation team.
- Level of programming skills required. More programming will increase the cost and is difficult to maintain the code.
- Level of skills and experience required for automation or maintenance.
- Security and data privacy. For example, security will have to perform a risk assessment of the tool for a secure environment.
- Time available to implement the TAS.
- Supplier’s financial solvency, to avoid investing in a tool supplier that may go bankrupt or struggle to keep on developing features.

3.3 CODING OR SCRIPTING

Coding or scripting is one of the essential factors in choosing the right tool for automation. Automated testing and test frameworks are software products, and they inevitably require coding or scripting. Coding enhances the effectiveness of the test automation tool and automated testing.

The following factors need to be considered before choosing the right test automation tool for your needs:

- Programming language used to develop the test automation tool
- Test automation tool compliance with the programming language used to develop the SUT

Coding or scripting can be applied in several different ways, such as in linear, structured, data-driven or OOP forms. This section covers different coding methods to be considered in the tool selection process.

3.3.1 Linear scripting

Linear test scripts are created while the user interacts with the application. The test actions mimic the actual user’s actions. Scripts are created in a ‘record and play’ format by capturing the user actions and system responses, recording them in an appropriate scripted format, and re-running them as required. They are linear because those steps through the application are performed sequentially.

3.3.2 Structured scripting

Structured scripting uses two tiers of the script. A high-level script outlines the basic steps and detailed procedural steps that perform the required subroutines. The test tool is programmed with a list of high-level tests to be run. During execution, these will automatically call the required low-level scripts.

3.3.3 Data-driven scripting

Data-driven scripting is where large volumes of data are used from separate data files for testing. The high-level script is created to read data items from the different data files. This reduces the script maintenance required per test.

3.3.4 Object-oriented programming

Object-oriented programming is widely known as OOP and is based on the concept of ‘objects’, which can contain data and code – data in the form of fields and code in the form of procedures. OOP implements entities like inheritance and polymorphism in programming and binds together data and functions. Python, Java, C++ and Ruby are a few examples of OOP-based languages.

3.4 SCRIPTLESS AUTOMATION

Scriptless or codeless test automation is performing test automation without writing any script or using limited scripts. Most of the widely used testing tools and frameworks provide this as a core feature, and this helps business users and manual testers to perform test automation without any or limited knowledge of programming languages. For example, scriptless automation can be used for validating the login functionality with a limited number of user accounts. However, human interaction or programming may be required, in this case, if the requirement is to validate the login for a large number of accounts. The scriptless feature enables testers and business users to automate test cases without coding skill. Codeless automation enables faster results and reduces the automation effort, and is suitable for many requirements. This is a key factor for test automation tool selection as in some cases, a scriptless tool is enough to meet the automation need.

Advantages of scriptless automation are:

- No dependency on programming languages and scripting as there is no coding involved
- More user engagement from non-technical members or business users of the organisation as it requires no or minimum technical skills
- Easy to automate, quick turnaround and payback
- Reduced cost and effort

Disadvantages of scriptless automation are:

- Testing lacks depth and is not thorough as programming enhances the effectiveness of testing.
- No or less scope for customisation as the tools provide limited options to customise without coding.
- One hundred per cent codeless is difficult to achieve.

This book does not cover the details of how to programme or code as there are plenty of books and online resources available for learning coding/programming step-by-step.

3.5 SUMMARY

In this chapter, we addressed the significance of the role of testing tool selection, selection criteria and coding methods to influence the tool selection. Tool selection is an important factor for the success of automation. Knowledge of coding methods is also a key factor for the successful definition of the ideal test automation framework. In the next chapter, we will explore another important area: how to build a test automation team.
