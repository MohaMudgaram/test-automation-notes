## SAMPLE TEST AUTOMATION FRAMEWORK

> Reference Book:
> 
> Test Automation
> 
> By Boby Jose

---

Figure A.1 shows a sample framework created in Selenium and C# programming language for an ecommerce application.

Figure A.1 Test automation framework folder structure

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/FigA-1.png)

The key folder details are provided in Table A.1 for the framework.

Table A.1 Test automation framework folder description

|                 |                                                                                                                                                                                                                                                                                                                                           |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Folders         | Description                                                                                                                                                                                                                                                                                                                               |
| Config          | Stores the information that remains static throughout the framework such as browser-specific information, application URL, screenshots path.                                                                                                                                                                                              |
| Extensions      | Extension Methods (C# Programming Guide): ‘Extension methods enable you to “add” methods to existing types without creating a new derived type, recompiling or otherwise modifying the original type. Extension methods are static methods, but they are called as if they were instance methods on the extended type’ (Microsoft, 2020). |
| Factory         | Driver Factory: ThreadSafe Driver for running parallel test execution.                                                                                                                                                                                                                                                                    |
| Browser Factory | This allows a browser instance to launch based on the parameter, and creates the webdriver object for the given browser.                                                                                                                                                                                                                  |
| Helpers         | Helper class is used for Date, FileType, Name and WaitHelper.                                                                                                                                                                                                                                                                             |
| Logger          | This module will log messages to test output.                                                                                                                                                                                                                                                                                             |
| Reports         | Extent Reports has been used in this case. It generates HTML reports and maintains logs to include the screenshots of failed test cases in the Extent Report.                                                                                                                                                                             |

Figure A.2 provides the framework shown in Figure A.1 used for a real-life project.

Figure A.2 Test automation framework for a real-life project

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/FigA-2.png)

The folder details are provided in [Table A.2 for the real-life project framework.

Table A.2 Test automation framework folder description for a real-life project

|         |                                                                                                                                                                                                                                                                                      |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Folders | Description                                                                                                                                                                                                                                                                          |
| AutoIt  | AutoIt v3 is a freeware like BASIC scripting language designed for automating the Windows GUI and general scripting. It uses a combination of simulated keystrokes, mouse movement and window/control manipulation in order to automate tasks, which are not possible with Selenium. |
| Config  | Configuration instance to get the values from the appSettings.json file.                                                                                                                                                                                                             |
| Model   | This is the model class for the appSettings file.                                                                                                                                                                                                                                    |
| Pages   | Holds the page object for the application. The framework creates a new folder for each project. Apart from Homepage all other pages will inherit from BasePage.                                                                                                                      |
| Reports | Extent reports are stored in the Reports folder. In this case it overwrites the file in each run.                                                                                                                                                                                    |
| Tests   | Stores all the tests.                                                                                                                                                                                                                                                                |

In this framework, the test cases were executed in a parallel run. The parallel execution helps to save time in test execution; for example in a normal scenario, if it requires 100 minutes to run 100 tests, in parallel execution if five threads are used at the same time, it takes only 20 minutes to run 100 tests (100/5 = 20) (Figures A.3 and A.4).

Figure A.3 Test automation framework test result 1

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/FigA-3.png)

Figure A.4 Test automation framework test result 2

![images](https://learning.oreilly.com/api/v2/epubs/urn:orm:book:9781780175478/files/Images/FigA-4.png)
