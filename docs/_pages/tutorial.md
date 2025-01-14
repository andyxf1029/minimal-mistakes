---
title: "Tutorial"
permalink: /tutorial/
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



<figure>
  <img src="{{ '/assets/images/Last-Hit-WelcomePage.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


<figure>
  <img src="{{ '/assets/images/Last-Hit-CreateWorkspace.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>



Step 2: Click the Create New One on left frame to create new story(test case). Provide a name for your story and click OK. An empty story will be created.

<figure>
  <img src="{{ '/assets/images/Last-Hit-CreateNewStory.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Step 3: click the Create New One on left frame to crate new flow(set of test step). Provide a name for your flow and click ok. An empty flow will be created.

<figure>
  <img src="{{ '/assets/images/Last-Hit-CreateNewFlow.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Step 4: Click Record from the main toolbar.

<figure>
  <img src="{{ '/assets/images/Last-Hit-ClickRecordButton.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Step 5: Provide Start Url and Device whick you wanted, click Ok.

<figure>
  <img src="{{ '/assets/images/Last-Hit-StartRecordDialog.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Step 6: Once your application has been launched, you will be directed to the Login page. Enter valid username and password, then click Login.

<figure>
  <img src="{{ '/assets/images/Last-Hit-Recording.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Step 7: Now we have finished this flow, click Stop from the main toolbar to finish recording.

<figure>
  <img src="{{ '/assets/images/Last-Hit-StopRecording.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Step 8: Click Stop close Chromium.

<figure>
  <img src="{{ '/assets/images/Last-Hit-StopRecordDialog.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>




Step 9: Now you can just click Play to execute recorded test cases in your chromium. It's as simple as that

<figure>
  <img src="{{ '/assets/images/Last-Hit-StartReplay.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>



The story and flow scripts whick you recorded and replay will store in your worksapce with json file.


<figure>
  <img src="{{ '/assets/images/Last-Hit-Script.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


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

<figure>
  <img src="{{ '/assets/images/Last-Hit-WorkspaceWholePicture.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>



# Workspace

<figure>
  <img src="{{ '/assets/images/Last-Hit-Workspace.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


*New Story*

<figure>
  <img src="{{ '/assets/images/Last-Hit-NewStoryButton.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Create an new empty story for recording test case.

*Search Flow*

<figure>
  <img src="{{ '/assets/images/Last-Hit-SearchFlowButton.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Search the flow which you wanted.

*Enviroments*

<figure>
  <img src="{{ '/assets/images/Last-Hit-EnviromentsButton.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


Config env variables for record and replay 

*Workspace Settings*

Configure the workspace as you request

<figure>
  <img src="{{ '/assets/images/Last-Hit-WorkspaceSettingsButton.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>


# Toolbar

<figure>
  <img src="{{ '/assets/images/Last-Hit-Toolbar.png' | relative_url }}" alt="teaser image example">
  <!-- <figcaption>Example of teaser images found in the related posts module.</figcaption> -->
</figure>

<table><thead><tr><th>Icon</th><th>Description</th></tr></thead><tbody><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-SmartReplayButton.png' | relative_url }}" alt="teaser image example"></p></td><td>Smart to replay test case</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-ReplayButton.png' | relative_url }}" alt="teaser image example"></p></td><td>Start to replay test case</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-StepByStepReplayButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Replay test case step by step</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-StopReplayButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>When replaying test case step by step, stop replaying</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-RecordButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Start to record test case</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-RecordPauseButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Pause recording.</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-StopRecordButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Stop Recording</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-ShowAllStepButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Display all steps include request</td></tr></tbody></table>


# Step
![](/docs/_docs/media/tutorial/Last-Hit-StepToolBar.png)

<table><thead><tr><th>Icon</th><th>Description</th></tr></thead><tbody><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-AssertionButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Performace assertion after the step execution in replaying</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-ConditionButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Perform condition check before the step exection in replaying</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-BreakpointButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Add breakpoint on the step</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-MoveUpButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Move up the step</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-MoveDownButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Move down the step</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-MoveFreeButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Move the step freely</td></tr><tr><td><p>
<img src="{{ '/assets/images/Last-Hit-DeleteButton.png' | relative_url }}" alt="teaser image example">
</p></td><td>Delete the step</td></tr></tbody></table>


# CI Integration

how to run it in nodejs

CI report

code coverage

how to run it in jenkins

# Exception

how to find issue log and send to us

# Last-Hit Roadmap

![](/docs/_docs/media/tutorial/Last-Hit-FunctionRoadmap.png)

