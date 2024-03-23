## TEST AUTOMATION AND PROGRAMMING LANGUAGES

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

In the last chapter, we covered leading automation tools, their features and various costs involved in procuring and setting up these tools. Customisation of these tools makes them more suitable for organisational needs, and programming is required for customisation. In this chapter, we will explain programming and scripting in test automation at a high level and introduce you to some leading programming languages. These languages will help you in utilising most of the tools described in the previous chapters and creating scripts for specific needs. This chapter is not intended to explain how to do programming. Its purpose is an introduction to automated testing and programming languages. This chapter also addresses coding techniques and candidates for test automation.

Coding, scripting and programming are used to represent the same activity in automated testing.

Coding means using a computer language to create a set of instructions for the computer to behave as desired.

Scripting creates a set of commands that automates the execution of tasks. Scripting languages are often interpreted rather than compiled. Scripting languages are used to create scripting instructions.

Programming comprises a set of commands to produce a list of outputs. Programming languages are used to create programming instructions and implement algorithms.

A set of codes form a script, and a set of scripts form a program.

Programs need compiling before running, whereas scripts need interpretation. Compiled programs generally run swifter than interpreted programs as they compile a code in a complete set, and an interpreter interprets it line by line.

Scripting languages are usually coded in one language and interpreted within another program; for instance, JavaScript is included within HTML webpages and is interpreted by the web browser. Scripting languages are less code-intensive as compared to programming languages. In general, there is a difference between programming and scripting, but they are similar in many ways and hard to differentiate.

Programming languages are grouped into five different generations:

- First generation languages (1GL), for example machine-level programming languages
- Second generation languages (2GL), for example assembly languages
- Third generation languages (3GL), for example C, C++, Java and JavaScript
- Fourth generation languages (4GL), for example Perl, PHP, Python, Ruby and SQL
- Fifth generation languages (5GL), for example Mercury, OPS5 and Prolog

Figure 11.1 Generations of programming languages

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig11-1.png)

Scripting languages are grouped into two categories:

- Server-side scripting languages
- Client-side scripting languages

Most of the widely used automation tools use programming along with scripting for automated testing. Scripting is extensively used in non-functional automated testing, such as build validation. Perl, Python, Ruby, C# and Java are examples of programming languages, and Jscript is an example of a scripting language.

Good knowledge of programming and scripting is essential to be successful in automated testing.

11.1 PROGRAMMING LANGUAGES FOR TEST AUTOMATION

This section describes the key features of some leading programming and scripting languages used for test automation, with the aim of introducing you to different programming languages that can support the test automation need for your product or organisation.

Automated testing requires proficiency in programming languages and automation frameworks. The first step is to ensure that the SUT, test automation tool for automation and the programming skills in the test team are aligned. The commonly used programming languages to assist in test automation and their key characteristics, which are covered in this section, are:

- Python
- Perl
- Java
- C# (.Net)
- Ruby
- PHP
- JavaScript

11.1.1 Python

This section covers the popular programming language Python and some key characteristics of Python that support test automation:

- Python is a highly popular and extensively used open-source programming language for test automation.
- The syntax is considered easy to learn, and there is a strong presence of Python community at various technical levels, including end-users and programmers.
- Taught in the school curriculum in many countries, which creates a large pool of technical resources with good knowledge of Python coding.
- Python libraries reduce the amount of code writing necessary.
- High portability for the SUT and test automation suites developed in Python and it is compatible with many operating systems.
- Selenium and Appium libraries are available for Python.

11.1.2 Perl

This section covers Perl and some key characteristics of Perl that support test automation:

- Perl is an open-source and commonly used language for test automation.
- It is ideal for web programming, encryption and there are web-specific modules available in Perl.
- Highly recommended for GUI development and system administration.
- Supports object-oriented, procedural and functional programming.
- Perl supports text manipulation, Unicode and is quickly extendible.
- Used for embedded programming.
- Database integration and C/C++ library interface available in Perl.

11.1.3 Java

This section covers the object-oriented programming language Java and some key characteristics of Java that support test automation:

- Java is owned by the Oracle Corporation.
- It is extensively used and accepted within the development community.
- JUnit is a popular unit testing framework based on Java and is compatible with the Selenium testing tool.
- Many open-source test automation frameworks are developed using Java.
- Java follows the ‘Write Once, Run Anywhere’ principle, and it provides cross-platform compatibility.

Write Once, Run Anywhere (WORA) or Write Once, Run Everywhere (WORE) was a slogan created by Sun Microsystems to highlight the cross-platform benefits of the object-oriented Java programming language. It is the ability of the programming language to run on most common operating systems (OSs) without any changes.

11.1.4 C#

This section covers the C# language and some key characteristics of C# that support test automation:

- C# is based on object-oriented programming, created and supported by Microsoft Corporation.
- Extensively used for test automation and is a popular language using the .NET framework.
- C# is well suited for SUT based on Android, iOS, Windows and macOS platforms.
- It is compatible with Selenium testing tools and is effective for cross-browser testing.
- There are many test automation frameworks available in C#.

11.1.5 Ruby

This section covers Ruby and the key features of Ruby that support test automation:

- Ruby is an open-source language and is used for test automation of web applications.
- Ruby is popular among the student community due to its friendly syntax and flexible object-oriented architecture.
- It is popular for automated browser testing and considered easy for learning and implementing.
- It is compatible with the Selenium testing tool and is effective for cross-browser testing.

11.1.6 PHP

This section covers the PHP language and some key characteristics of PHP that support test automation:

- PHP is a server-side scripting language and is used for web development.
- It is used to manage dynamic content, databases, session tracking and so on.
- It is widely used in test automation.
- It is integrated with popular databases, such as Oracle and Microsoft SQL Server.
- There is active user community support available for PHP.
- PHP is embedded in HTML.

11.1.7 JavaScript

This section covers the scripting language JavaScript (JS) and some key characteristics of JavaScript that support test automation:

- JavaScript is a popular accepted scripting and markup language. It is used for front-end development and testing.
- It is commonly used for automated testing, and there are a wide range of test automation frameworks available in JavaScript.
- JavaScript, along with Selenium, is extensively used for automated browser testing.

11.2 CODING OR SCRIPTING METHODS AND TECHNIQUES

In the previous section, we addressed different programming languages commonly used for test automation and coding. Test automation inevitably requires the use of scripting to enhance the test scripts. Coding and scripting can be used in several different ways, and this section describes coding and scripting at a high level. Each of the methods in this section has its own advantages and disadvantages.

11.2.1 Linear scripting

In linear scripting, the test actions mimic the actual user actions that would be performed while using the application. These scripts are usually generated by a tool that provides a ‘capture and replay’ facility. This performs by capturing the user actions and system responses and recording them in an appropriate scripted format. The scripts can then be re-run for testing the SUT.

Advantages:

- Linear scripting requires minimal technical knowledge – The initial learning effort and development effort is low and can be introduced very quickly.
- No programming skills are required since it is click and record – This helps the non-technical business users perform linear scripting.
- Most of the test automation tools provide ‘capture and replay’ and an inbuilt feature.

Disadvantages:

- The scripts capture all the user actions, including any incorrect ones.
- The script may become inefficient due to repetitive user actions, for example repeated browser back button usage.
- The tests are dependent on the user interface as any minor changes in the user interface will halt further tests.
- The scripts are only applicable to the recorded set of actions and cannot be used elsewhere.
- The linear scripts lack error and exception handling, and any failure in test execution will stop the remaining tests.
- Any change to the SUT may impact all the test scripts, and all the recorded scripts may need to be updated.
- Some record and replay tools use proprietary scripting language; this can make the script difficult to understand, maintain and modify.

11.2.2 Structured scripting

Structured scripting is widely used for coding and test automation. In structured scripting, existing tests are used as the basis for creating two-tier test automation scripts. The first tier is a high-level script outlining the basic steps. The second-tier scripts are more detailed procedural steps that perform the required subroutines. The test tool is programmed with a list of high-level tests to be run. During execution, these will automatically call the required low-level scripts. This is illustrated in the below figure.

Figure 11.2 Structured scripting

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/Fig11-2.png)

Advantages:

- The control scripts are structured in two levels and are easy to understand, execute and maintain.
- It is easy to define and develop the second tier and other variants of tests once the initial scripts have been created.
- The shared scripts can reduce maintenance costs.

Disadvantages:

- More effort is required, at the beginning, to design and set up the main and shared scripts.
- Greater technical and programming skills are required compared to linear scripting.
- The script library must be well maintained for future enhancement.

11.2.3 Data-driven scripting

Data-driven scripting is an extension of the structured scripting explained in the previous section, and is where data values are embedded into the high-level scripts. Data files can be stored in a spreadsheet or a database.

Data-driven scripting can lead to many scripts to achieve the required set of tests for range testing. It is a further extension to structured scripting to extract the required data into separate data files. The high-level control script is modified in order to read data items from the data file. Therefore, one script can implement several tests by reading data from different data files. This reduces the script maintenance required per test.

Advantages:

- Reduced build costs since it is faster and easier to build similar test procedures.
- Easy to create many variations of the basic test but using different data.
- The external data file can be created and maintained by the business as this provides an additional guarantee to the test automation coverage.

Disadvantages:

- More initial effort is required to ensure the various files will all operate together correctly (and to meet future needs).
- More initial effort is required to program the main and low-level test scripts.
- Requires a higher level of programming skills.

11.3 CANDIDATES FOR TEST AUTOMATION SCRIPTING

It is rarely feasible to automate all test cases and tests, as some tests will be difficult to automate or will return low benefits when compared to the effort required. This section lists a set of questions to be asked before selecting the tests, feasibility of features and identifying requirements for test automation.

- Is the test case repeatable? It is good for automation if it is used very often. Tests used once or infrequently are not suitable for automated scripting as the ROI will be low.
- Does the test require any manual intervention? If the tests require manual intervention to complete they are not a good candidate for automation, for example many scientific applications.
- Could all test preconditions be set up automatically? If so, this is a good candidate as it requires less manual intervention, for example setting up test data automatically for testing.
- Are the expected results dynamically changing? These tests are difficult to automate and require a lot of scripting and coding effort, for example **Global Positioning Systems (GPSs)**.
- Does the SUT change dynamically, for example using data feeds? They are difficult to automate because the expected result changes constantly, and successful implementation requires a lot of effort, for example accessing the data feed at the source to match with the result on the front end.
- How easy is it to set up test data for the test case? In some cases, test data need to be set up manually. This will increase the effort for test preparation, reduce the reuse of automated testing and the ROI will be low for test automation.
- Are they UI/UX tests? User experience, also known as ‘look and feel’, tests require manual intervention to validate the results and are difficult to script. They are not considered good candidates for automation.
- Could a clear pass or fail criterion be defined? It is important for the tool to validate the actual result against the expected result. It is difficult to script dynamically changing or ambiguous outcomes for the same inputs. Many test automation tools provide tolerance in the expected result. However, this can impact the accuracy of the testing.
- Could the test case be manually validated with less effort? These tests may not be good candidates for test automation as scripting and test automation delivers a lower ROI compared to manual testing.
- How quick would it be to update the test if the system functionality changes? This is a key factor for scripting as it takes a lot of effort to maintain the scripts.
- Is it difficult to code or script? Avoid these tests as automated scripts can be ‘flaky’ and difficult to debug.

A test script is a set of instructions for automated testing using a scripting or a programming language.

11.4 DEVELOPING YOUR FIRST SCRIPT

A systematic and disciplined approach is always useful for test automation and automated testing. It is difficult to introduce all the automation in a single exercise, and easier to introduce automation in a number of disciplined steps and stages. This section provides a set of examples to commence test automation, automate the first script and extend the first script to a test automation suite.

- Example one. Start with a simple record–replay tool to create an initial set of automated scripts and then use scripting or coding techniques to enhance the ‘record and replay’ script to develop a more powerful script; for example enhance the ‘record and replay’ to a data-driven script and develop a test suite that can be used for validating a large volume of inputs.
- Example two. Using an existing automation framework or suite helps in building the automation experience slowly and avoids delivery pressure. Extending the framework libraries or adding new automated tests to an existing framework supports the learning process.
- Example three. Start with a SUT that is in a more stable phase, for example a maintenance phase, where a large number of regression tests might be the first candidates for scripting and test automation.
- Example four. Start with an existing product for developing the first script for test automation as the SUT changes are minimal.

Below there are a few alternative options to commencing test automation if support from the leadership and organisation are minimal because of other priorities and commitments.

- Open-source tools
- Record and playback
- Existing test suite

11.4.1 Open source

The automated script needs to be reliable, robust, maintainable, easy to debug and scalable to multiple environments. Open-source tools are a good option as they are cost-effective, require minimum hardware or infrastructure and have massive support available from the community. The first step to using open-source tools is to download the tool, install it and select a simple functionality to automate. Most of the open-source tools and languages provide a beginners’ guide to starting automation.

11.4.2 Record and playback

Record and playback is another way to introduce test automation in the organisation. It is a type of automated testing where the tool records the activity of the user and then imitates it while playing back. Most of the widely used tools and frameworks support this feature. Record and playback provide a basic script, which can be enhanced, for example a simple record and playback script for login functionality can be enhanced with a data-driven approach to extend 100 per cent test coverage.

11.4.3 Existing test suite

Another good approach is to start with the existing regression pack. Many organisations and projects continuously use existing regression tests with minimal changes. Over a period, an automated regression pack becomes toothless and obsolete due to lack of maintenance, although part of these scripts can be useful after modification. The obsolete regression pack is a good place to reintroduce automated testing cost-effectively.

11.5 SUMMARY

In this chapter we have looked at the role of programming or scripting languages and coding in test automation. Scriptless tools are now widely used; however, coding cannot be ignored as it enhances the ability of test automation. This chapter also discussed different coding methods and how to start automated testing if you are new in this area. This chapter helps test managers and Scrum masters to introduce test automation in their organisation.

The next chapter will cover test automation framework design and how to start with automating scripts. However, not all organisations and projects approach automation systematically and many organisations lack budgetary support for test automation. Nevertheless, test automation leaders can still introduce automation with minimal resource and budget support.
