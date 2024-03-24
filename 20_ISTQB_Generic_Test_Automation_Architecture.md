## ISTQB TEST AUTOMATION ARCHITECTURE

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

The gTAA was developed by the ISTQB as part of the TAE certification syllabus. The gTAA provides an approach to implementing TASs for software projects. gTAA is a widely used and popular test automation architecture for designing, developing, implementing, and maintaining TASs. The gTAA-designed test automation architecture has a structure of four horizontal layers, which are test generation, test definition, test execution, and test adaptation. These layers are supported by the management layers, such as test management, project management, and configuration management.

The TAE syllabus advises implementing the TAS in incremental steps (e.g. in sprints) for quick benefits with a recommendation of a proof of concept for test automation projects. The test automation project is generally managed as a software development project.

The gTAA is vendor independent and is often implemented by a set of tools and the components. The gTAA can be implemented by using any development approach, such as structured, object-oriented, service-oriented, or model-driven, as well as by any software technologies and tools. TAS is often implemented using off-the-shelf or open source tools but often needs additional SUT-specific additions and/or adaptations.

The test generation layer is generally used for designing test cases, and the test definition layer supports the definition and implementation of test suites or test cases. The test execution layer provides an execution tool to run the tests automatically along with a reporting component. The test adaptation layer helps the code to adapt the automated tests for various SUT components or interfaces. It provides different adaptors to connect with the SUT via APIs, protocols, services and so on.

The most common and popular test automation tools are suitable for implementing gTAA. The test automation planning and PoC stages are appropriate places to identify the components and layers of the gTAA required for your solution. The TAE syllabus provides suggestions about how to use a gTAA-based approach in an Agile and DevOps environment.

The gTAA is largely described as a monolith as it is composed of all its components in one architecture. The monolithic framework/application/architecture describes a single structure in which different components are combined into a single platform or a framework. Components can be business logic, database layer, API layer, or application integration and so on.

Figure A.7 The Generic Test Automation Framework ©International Software Testing Qualifications Board (ISTQB), 2016

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/FigA-7.png)
