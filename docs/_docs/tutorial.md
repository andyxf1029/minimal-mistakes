---
title: "Tutorial"
permalink: /docs/tutorial/
excerpt: "How to use last-hit for web automation testing"
last_modified_at: 2019-10-02T13:34:11-04:00
redirect_from:
  - /theme-setup/
toc: true
---

# Welcome to Last-Hit
last-hit is a simple and powerful automation solution. It revolutionizes the use of open-source frameworks such as electron and puppeteer by eliminating their technical complexities to allow developers and QAs to efficiently set up, create, run, report, and manage their automated tests.

# Tutorial
Last-Hit team has some sample projects and documents for you to try out before testing out your own products. The Learning Center hosts tutorials for you to follow along and get to know last-hit features

# Last-Hit Documentation
Our documentation will help you with configurations, features utilization and important information to create a successful automation test.

Test Case contains information on various components of a test case/test suite. Here, you can read more about last-hit features that will assist you during test case construction. 

After designing a test, Execution shows you how to run your test cases/test suites. Before executing your tests, keep in mind last-hit's supported execution environments.

Reports provides a comprehensive view of your test results. You can also utilize our beta product, Last-Hit Management(coming soon), for manage and analysis of the test reports.

# Support
The Last-Hit Community with fellow users and experts will help you with any issues while utilizing Last-Hit. Some issues, however, are documented here, which the Last-Hit team has planned to fix and improve in future releases. 

You can also suggest new features for Last-Hit and Last-Hit Mangement in the forum. The Last-Hit team are eager to see your suggestions to make our product better for our community.

# Introduction to Web Testing
This is a basic tutorial about how to begin testing with Last-Hit. If you are completely new to Last-Hit or have just begun testing with the app, this ‘Getting Started’ doc is for you. We will go over a few principal steps, basic concepts, and operations in Last-Hit. You will learn how to create projects, create, verify, debug, as well as successfully plan and execute test cases.

# Creating test cases using Record & Playback
Test recording is the easiest way for new automation testers to start learning test automation. Identifying objects on applications is time-consuming. The Web Recorder Utility function captures your actions being performed on the application and converts them into runnable code in the back-end.

You can quickly automate a few functionalities of your app and save time by recording actions that have to be performed many times in iterative builds. This function supports recording and running the same tests on chromium. This document will show you how to:

    1. Record test with the Record Web function.
    
    2. Replay test with the reocrd script.

Record Test with the Record Web function

**Scenario**: To Login

    1. Launch the application under test (Example: https://github.com/login)

    2. Enter a valid username, password, and click Login
    
    3. Login successfully

Follow the below steps to get familiar with the Record & Playback feature for Web UI tests

Step 1: Launch Last-Hit and click Create New Workspace on the main screen. Provide a name and location for your workspace and click OK. An empty workspace will be created.

![](/docs/_docs/media/tutorial/Last-Hit-WelcomePage.png) 

![](/docs/_docs/media/tutorial/Last-Hit-CreateWorkspace.png) 

Step 2: Click the Create New One on left frame to create new story(test case). Provide a name for your story and click OK. An empty story will be created.

![](/docs/_docs/media/tutorial/Last-Hit-CreateNewStory.png)

Step 3: click the Create New One on left frame to crate new flow(set of test step). Provide a name for your flow and click ok. An empty flow will be created.

![](/docs/_docs/media/tutorial/Last-Hit-CreateNewFlow.png)

Step 4: Click Record from the main toolbar.

![](/docs/_docs/media/tutorial/Last-Hit-ClickRecordButton.png)

Step 5: Provide Start Url and Device whick you wanted, click Ok.

![](/docs/_docs/media/tutorial/Last-Hit-StartRecordDialog.png)

Step 6: Once your application has been launched, you will be directed to the Login page. Enter valid username and password, then click Login.

![](/docs/_docs/media/tutorial/Last-Hit-Recording.png)

Step 7: Now we have finished this flow, click Stop from the main toolbar to finish recording.

![](/docs/_docs/media/tutorial/Last-Hit-StopRecording.png)

Step 8: Click Stop close Chromium.

![](/docs/_docs/media/tutorial/Last-Hit-StopRecordDialog.png)

Step 9: Now you can just click Play to execute recorded test cases in your chromium. It's as simple as that

![](/docs/_docs/media/tutorial/Last-Hit-StartReplay.png)

The story and flow scripts whick you recorded and replay will store in your worksapce with json file.

![](/docs/_docs/media/tutorial/Last-Hit-Script.png)

Scripts is in a very clear and readable format, you can read the JSON file to see the detailed steps of the test case.

```json
{
	"description": "",
	"steps": [
		{
			"type": "start",
			"url": "https://github.com/login",
			"device": {
				"name": "iPad",
				"userAgent": "Mozilla/5.0 (iPad; CPU OS 11_0 like Mac OS X) AppleWebKit/604.1.34 (KHTML, like Gecko) Version/11.0 Mobile/15A5341f Safari/604.1",
				"viewport": {
					"width": 768,
					"height": 1024,
					"deviceScaleFactor": 2,
					"isMobile": true,
					"hasTouch": true,
					"isLandscape": false
				}
			},
			"uuid": "75714aa0-1efa-4d19-81a5-9144a58d8bdd"
		},
		{
			"detail": 0,
			"isTrusted": true,
			"path": "//*[@id=\"login_field\"]",
			"scrollLeft": 0,
			"scrollTop": 0,
			"target": "<input type=\"text\" name=\"login\" id=\"login_field\" class=\"form-control input-block\" tabindex=\"1\" autocapitalize=\"off\" autocorrect=\"off\" autofocus=\"autofocus\">",
			"timeStamp": 4513.0450000287965,
			"type": "focus",
			"uuid": "75714aa0-1efa-4d19-81a5-9144a58d8bdd",
			"value": ""
		}
    ]
}
```

# What cannot be recorded?
To do?

# GUI
Last-Hit 

![](/docs/_docs/media/tutorial/Last-Hit-WorkspaceWholePicture.png)


# Workspace

![](/docs/_docs/media/tutorial/Last-Hit-Workspace.png)

New Story -

Search Flow -

Enviroments -

Workspace Settings -



# Record
![](/docs/_docs/media/tutorial/Last-Hit-RecordToolBar.png)

Start record - 

Pause record -

Stop record -


<table><thead><tr><th>Icon</th><th>Description</th></tr></thead><tbody><tr><td style="text-align:center"><p><img src="https://github.com/andyxf1029/minimal-mistakes/blob/master/docs/_docs/media/tutorial/Last-Hit-RecordButton.png"></p></td><td>Save the current opened test artifact.</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A193A17.png"></p></td><td>Save all opened test artifacts.</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A183A47.png"></p></td><td><p>Create new test artifacts. You can select these options by selecting from dropdownlist:</p><ul><li>Folder</li><li>Test Case</li><li>Test Suite</li><li>Test Suite Collection</li><li>Test Object</li><li>Web Service Request</li><li>Test Data</li><li>Checkpoint</li><li>Package</li><li>Keyword</li></ul></td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A203A11.png"></p></td><td>Open <strong>Web</strong> <strong>Object Spy</strong> dialog for capturing elements on websites.</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A203A32.png"></p></td><td>Open <strong>Mobile Object Spy</strong> dialog for capturing elements on mobile applications.</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A213A15.png"></p></td><td>Open <strong>Web</strong> <strong>Record</strong> dialog for recording WebUI test cases.</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A203A56.png"></p></td><td>Open <strong>Mobile Recorder</strong> dialog for recording Mobile test cases.</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A213A34.png"></p></td><td><p>Run the current open test case. You can select these options by selecting from dropdownlist:</p><ul><li>Chrome</li><li>Firefox</li><li>IE</li><li>Safari</li><li>Edge</li><li>Remote</li><li>Headless</li><li>Android</li><li>iOS (on macOS)</li><li>Custom</li></ul></td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A223A4.png"></p></td><td><p>Debug the current open test case. You can select these options by selecting from dropdownlist:</p><ul><li>Chrome</li><li>Firefox</li><li>IE</li><li>Safari</li><li>Edge</li><li>Remote</li><li>Headless</li><li>Android</li><li>iOS (on macOS)</li><li>Custom</li></ul></td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A223A28.png"></p></td><td>Stop the current execution</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A223A45.png"></p></td><td>Open <strong>Command Builder</strong> for generating commands for console execution</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A233A4.png"></p></td><td><p>Command for Git activities. You can select these options by selecting from dropdownlist (after <a class="external-link" href="/display/KD/Git+Integration" rel="nofollow">enabling Git</a>):</p><ul><li>Clone Project</li><li>Share Project</li><li>Show History</li><li>Manage Branches</li><li>Commit</li><li>Push</li><li>Pull</li><li>Fetch</li></ul></td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-16-183A233A24.png"></p></td><td>Import test case from JIRA integrated account</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-4-3-153A93A34.png"></p></td><td>Execution profile (testing environments) to be applied when run tests</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-8-1-113A263A34.png"></p></td><td>Allowing you to search for help on Katalon Documentation and our Forum</td></tr><tr><td><p><img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/toolbars-and-views/image2018-8-1-143A93A36.png"></p></td><td>If you have any further questions, you can also submit it in our Gitter channel. Katalon experts and users will try to help you as soon as possible.</td></tr></tbody></table>


# Replay
![](/docs/_docs/media/tutorial/Last-Hit-ReplayToolBar.png)

Smart play -

play -

Step by step - 

# Step
![](/docs/_docs/media/tutorial/Last-Hit-StepToolBar.png)

Assertion - 

Condition -

Breakpoint - 

Move up -

Move down -

Free Move - 

Delete -

# CI Integration

how to run it in nodejs
CI report
code coverage
how to run it in jenkins

# Exception

how to find issue log and send to us

