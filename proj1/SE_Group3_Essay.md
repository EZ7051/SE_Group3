**CSC 510 Software Engineering Project-1**

**Group - 3**

**Team members:**

**Name Unity ID**

Ejaz Ahamed Shaik eshaik

Shynitha Muthyam smuthya

Soubhagya Akkena sakkena

Sumalatha Mashetty smashet

**Github repository**:[ ](https://github.ncsu.edu/araveen/engr-ALDA-Fall2022-H35)[https://github.com/EZ7051/SE_Group3 ](https://github.com/EZ7051/SE_Group3)</br>
We got 5 projects and after trying to run all of them, we made two of our applications run successfully after many modifications, errors and installations. Out of those two we found the ‘Cheapbuy’ project needs little grooming. So we, Team - 3 chose ‘Cheapbuy’ as our project 2 to make the application run seamlessly and to make it available for everyone. We also jotted down in this documentation, the problems and errors we faced during the process and how we overcame them. This documentation also includes a few points on how we can avoid those pains in our upcoming projects.


- What was hard about the process :
    - While installing the requirements file encountered many version incompatibility issues like below :



ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.

xarray 2022.11.0 requires pandas>=1.3, but you have pandas 1.1.5 which is incompatible.

jupyterlab-server 2.19.0 requires requests>=2.28, but you have requests 2.26.0 which is incompatible.

conda-repo-cli 1.0.27 requires clyent==1.2.1, but you have clyent 1.2.2 which is incompatible.

conda-repo-cli 1.0.27 requires nbformat==5.4.0, but you have nbformat 5.7.0 which is incompatible.![](Aspose.Words.6da1bd32-516e-4fbd-8b3e-a99145b1e0f0.002.png)

conda-repo-cli 1.0.27 requires requests==2.28.1, but you have requests 2.26.0 which is incompatible.

black 22.6.0 requires click>=8.0.0, but you have click 7.1.2 which is incompatible.


     - Some of the components were not mentioned in the requirements.txt file which would only work with a specified version. Like flask==2.1.2, protobuf==3.20.0, altair==4, and updating webdriver\_manager to the latest version in case of the cheap buy application.
     - Below are the errors for the same :



TypeError: Descriptors cannot not be created directly.

If this call came from a \_pb2.py file, your generated code is out of date and must be regenerated with protoc >= 3.19.0.

If you cannot immediately regenerate your protos, some other possible workarounds are:

1. Downgrade the protobuf package to 3.20.x or lower.
1. Set PROTOCOL\_BUFFERS\_PYTHON\_IMPLEMENTATION=python(but this will use pure-Python

parsing and will be much slower).

ModuleNotFoundError: No module named 'altair.vegalite.v4'

Exception in thread... There is no such driver by url https://chromedriver.storage.googleapis.com/LATEST\_RELEASE\_116.0.5845


       - In certain projects, the documentation isn't precise or thorough enough, especially when it comes to error management and resolution techniques. This shortcoming might make it difficult for users to troubleshoot problems successfully, making it essential to improve documentation by offering precise, thorough, and useful advice for fixing errors.
      - In one project, the absence of a requirements.txt file posed significant challenges during installation, creating difficulties due to unclear dependencies.
      - One of the projects was not working on an outdated library so we had to update the corresponding library which included additional code changes. Also, some of the libraries were deprecated / no longer supported by the system.
      - One of the projects did not mention the installation and setup instructions clearly which made the whole process tedious. For example, the database connection script wasn’t mentioned.
      - In one of our projects, we encountered a situation where some of the components and modules they had utilized were no longer compatible with the latest versions. Consequently, we were unable to successfully execute the project using the current software versions, leading us to downgrade these components to earlier versions in order to maintain functionality.
      - In one of the projects, proper test cases were not provided, thus the boundary conditions were left out.
      - Some projects did not have proper API documentation. It was difficult to understand the functionalities of the API.
      - Some of the videos could not capture all the aspects of the functionalities of each module
- How can you avoid it and what practices are you committing to perform in project2 to avoid that pain:
    - We need to make sure that all the components are mentioned inside the requirements.txt file with the proper versioning.
    - To enhance user support, creating a set of FAQs addressing common beginner errors encountered during application installation can be invaluable, offering quick solutions and improving the overall user experience.
    - In our documentation, it's essential to incorporate information about potential errors and their solutions to assist users in effectively troubleshooting issues they may encounter.
    - Stay informed about updates and changes in the libraries and tools you use. Regularly check for new releases and release notes to anticipate potential compatibility issues.
    - We are committed to ensuring that our software's website and documentation offer a transparent, comprehensive, and concise overview of the software's features and functionality, facilitating user understanding and engagement.
    - Before merging changes or adding new dependencies, conduct peer reviews to ensure that everyone on the team is aware of and approves these modifications, minimizing the risk of unexpected compatibility problems.
    - You can containerize the application using Docker to mitigate version incompatibility problems.
    - Continuously test the project on various platforms and environments to identify and resolve compatibility issues before they become major roadblocks.
    - Implement a CI/CD pipeline that automatically builds and tests the project with different configurations. This can help catch compatibility issues early in the development process.
    - Commit to providing thorough and clear documentation for the project. Include step-by-step instructions for setting up the environment, running the application, and troubleshooting common issues. Document any potential pitfalls and their solutions.
    - In one of the projects, the code coverage was just 35%. Maintaining high code coverage is essential for quality assessment of code.
    - Aim to develop a comprehensive suite of unit test cases for our code that cover various code paths and scenarios.
    - Provide effective API documentation that gives clear and concise descriptions for each endpoint, including what it does and how to use it. Effective API documentation is essential for ensuring that developers can quickly and accurately implement the API into their projects.
