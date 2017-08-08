# Project NASA XYZ


## How to setup and run:
To run tests please do the following:

1. First download & install latest Java into your machine following the link
   `http://www.oracle.com/technetwork/java/javase/downloads/index.html`
   
2. Also download & install Maven into your local machine following the link
   `https://maven.apache.org/download.cgi`
    
3. Then clone this repository following the GIT workflow below

4. To run from command prompt navigate to the project location and type 
   "mvn clean test -Dmaven.surefire.debug -U -DforkCount=0 -Dgroups=regression"


## Git Workflow:

1. Download and install Git from:  `https://git-scm.com/downloads`
2. Clone the repository: `https://github.com/MuhammadAhsanullahII/projectnasaxyz.git`
3. Create new branch from the local repository: `git checkout -b <branch-name>`
4. Optional- create a remote branch to be always updated with latest changes `git push <remote-name> <branch-name>`
   Note: Some additional commands are necessary in order to contribute, commit, and push new tests to this project.


## About what the framework tests:
The project tests an API developed by NASA, pretty much thoroughly with positive and negative data and logs test results. The script make calls to the API using the test data, captures the response, converts the response and maps the schema objects, asserts on expected values, reports test failures.

The scenarios tested can be outlined mainly as happy path, boundary value analysis invalid data type, null and blank values, and some special characters. Kind of tests has been commented on the NasaApiTest.java class. Testdataset.json has all the different data passed in for the tests. Also the test scenarios and results are attached with the project as an excel attachment, please refer to "test scenarios and results.xlsx".


# Note: Very Important!!!
NASA restricts the number of calls made to the API under test, therefore, the automated test suite has limitation as IP being blocked due to "OVER_RATE_LIMIT"
