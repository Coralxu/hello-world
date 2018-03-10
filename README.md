# Test Plan


**Author**: Team 14

## 1 Testing Strategy

### 1.1 Overall strategy


1. **Unit Testing**: This testing will be action that we will use to validate different units 	of source code and make sure they remains working properly. we will perform this test/s cases on function, method, Loop or statement etc.

2. **integration Testing**:This testing will be an action that we will perform to make sure that individual software modules are combined and tested together as a group. This usually occur after unit testing. In more detail, we will take modules that have been unit tested, groups them in larger aggregates, applies tests defined in an integration test plan to those aggregates, and delivers as its output the integrated system ready for system testing

3.  **System Testing**: This is a testing that is conducted on a complete and integrated system to evaluate the system's compliance with its specified requirements. We will not ve performing system test for now.

4. **Regression-testing**:This is a software testing that ensures that the previous developed and tested software still performs the same way after it is changed or interfaced into another software.

### 1.2 Test Selection


We intend to used different techniques other than blackbox testing, we are going to do 3 different testing, this tests will help up with the assertion of the core requirments of the software. with this being said we will will be doing Unit test, which test the behavior of a function, method or statment, we will then do integration test which is the combination of different small functions as a group in a module and test the whole module as a 1. with this we can assert that the interaction bettwen smaller function that are suppose to work together work as expected. we will lastly then do regression testing this will enable use to make sure that previous working module or entity of the project that is being worked on due to some bug fixes or addition of functionlity to that module sill work as epected per requirements.  

### 1.3 Adequacy Criterion


Depending on what ide we intend to use. Majorly jetbrains Solutions, its ide comes with and extenstion that allows one to do a code coverage of a function of the unit test. With this criteria, the more the percentile of the code coverage analysis is presented the better the quaity the of the test cases

### 1.4 Bug Tracking

In this project, we are going to be using GIT. A version controll system which helps in the iterations of SDLC. we will be using git issues system to track issues/bug and enhancement request. this will help us manage and have a structured top to bottom approach on fixing bugs and/or enhancment request.

### 1.5 Technology

We intend in using Junit, Using Junit is a Java Unit testing framwork. This enables us to test for possible outcomes as expected from a function/method or statments. etc. we are able to test for Nullreference, Assetions of return values, inavlid arguments and many more. with this technology we are able to adopt a development approach called test driven development with will allow us to write all our test cases as per the requirement and we then write functoion and classes to match those cases.


## 2 Test Cases

| ﻿Test Cases              | Purpose                                                         | Steps to perform Test                                                                                                                                              | Expected Result                                                                                                | Actual result | pass/fail | Other result |
|-------------------------|-----------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|---------------|-----------|--------------|
| Application Start Up       | make sure App loads                        | Open App                                                                                                                 | App Opens|Open App |Pass
| Application Login Button      | Go to Login Screen                       | Click Login Button                                                                                                                | Goes to login screen                                                             |     Goes to login screen         |     Pass      |              |                                                               |     App Opens        |     Pass      |              |
|Logging in Success Message    | Logging in                      | Click Login and enter username                                                                                                               | Login in Success Message|Login in Success Message |Pass
|Logging in fail Message    | Logging in                      | Click Login and enter  wrong username                                                                                                               | Login in fail message|Login in fail Message |Pass
| For registration        | make sure player information is saved                           | check database to see if we can find this player                                                                                                                   | this new player should be found in the database                                                                |               |           |              |
| For creating puzzle     | make sure new puzzle information is saved                       | check database to see if we can find this new built puzzle                                                                                                         | This new puzzle should be in the database                                                                      |               |           |              |
| For creating tournament | make sure new tournament information is saved                   | check database to see if we can find this new built tournament and also the puzzles in this tournament                                                             | This new tournament should be in the database                                                                  |               |           |              |
| For playing puzzle      | make sure current puzzle game relation information is saved     | check database to see if we can find this puzzle game’s results.                                                                                                   | We should find all the results about this game by viewing statistics and also checking the database            |               |           |              |
|                         |                                                                 | such as player, puzzleID, score                                                                                                                                    |                                                                                                                |               |           |              |
| For playing tournaments | make sure current tournament game relation information is saved | check database to see if we can find this tournament game’s results.                                                                                               | We should find all the results about this tournament game by viewing statistics and also checking the database |               |           |              |
|                         |                                                                 | such as player, tournament name, the puzzles in this tournament, the score for each puzzle in this tournament, whether this tournament is completed by this player |                                                                                                                |               |           |              |
| Puzzle Statistics   for user          | display right puzzle statistics for user                                        | Poupulate the whole database   with seed data which follows the PK and FK constriants using Dao, and then   clicking the "PUZZLE COMPLETED" button | The right puzzle statistics   about this user should be shown                      | right statistics is shown                                               | pass |   |
| Tournament Statistics for user        | display right tournament statistics for user                                    | Poupulate the whole database   with seed data which follows the PK and FK constriants using Dao                                                    | The right tournament statistics   about this user should be shown                  | right statistics is shown                                               | pass |   |
| Puzzle Statistics for All             | display right puzzle statistics for all user                                    | Poupulate the whole database   with seed data which follows the PK and FK constriants using Dao                                                    | The right puzzle statistics for   all user should be shown                         | right statistics is shown                                               | pass |   |
| Tournament Statistics for All         | display right tournament statistics for all user                                | Poupulate the whole database   with seed data which follows the PK and FK constriants using Dao                                                    | The right tournament statistics   for all user should be shown                     | right statistics is shown                                               | pass |   |
| shown right format for puzzle phrase  | shown right format of puzzle   phrase before user starts playing game           | Junit test                                                                                                                                         | All the letters will be   substitute with "?", others will be shown                | right format of puzzle phrase is   shown before user start playing game | pass |   |
| update right format for puzzle phrase | update and shown right format of   puzzle phrase after user starts playing game | user start playing game by   clicking buttons to guess letters                                                                                     | The displayed format of puzzle   must be updated accordingly if user guesses right | right format of puzzle phrase is   updated                              | pass |   |
