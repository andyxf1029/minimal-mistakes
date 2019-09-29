---
title: "Quick-Start Guide"
permalink: /docs/quick-start-guide/
excerpt: "How to quickly install and setup Last hit for record and replay"
last_modified_at: 2019-08-20T21:36:11-04:00
redirect_from:
  - /theme-setup/
toc: true
---


# last-hit-quick-start

Last-hit is an automation testing solution aimed at development and operations teams.
It is focus on web test, gives you broad, deep and exact control over your web apps automation testing

A quick guide to set up and start your first automation test with last-hit, a free test automation tool built on top of electron and puppeteer. You now can begin automation testing on web & mobile with the least amount of effort. Free download at [site](www.last-hit.com).

Read [full guideline](https://last-hit.org/docs/tutorial/user-guide) here.

# Features:

- `Record` - Record to launch the browser. While recording, actions performed on the browser will be captured and generated into test steps.
- `Replay` - 
- `Parameterization` - 
- `Assertion` - 
- `Monitor` - 
- `Reporting` - 

You can learn more about each of these features within the [User Guide](https://last-hit.org/docs/tutorial/user-guide).

## To Use

To clone and run this repository you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
git clone https://github.com/last-hit-aab/last-hit.git
# Install dependencies
npm install
# Go into the repository
cd last-hit
# Install dependencies
npm install
# Go into the render folder
cd render
# Install dependencies
npm install
# Back to the root directory of repository
cd ../
# Run the app
npm run start
```

Note: If you want use Installation package, please download [Release Package](https://last-hit.org/release/download) or package by yourself. [How to package](https://last-hit.org/docs/tutorial/user-guide/howToPackage)

## Create your first Test Case

–  Select option to create new workspace from the main page

![](/assets/images/mainPage.png) 

–  Provide the name and location to create new workspace

![](/assets/images/mainPage2.png) 

–  Click [create new one] option to create new story.

![](/assets/images/workspacePage1.png) 

–  Provide the name for your story then click OK.

![](/assets/images/workspacePage2.png) 

–  A new story will be created accordingly. The story is also displayed. then click [create new one] option to create new flow.

![](/assets/images/workspacePage3.png) 

–  Provide the name for your flow then click OK.

![](/assets/images/workspacePage4.png) 

–  You can compose the flow by recording, replaying or manually editing test steps. For now, let's quickly generate the test script using Record feature. Click on the Record icon from the main Toolbar.

![](/assets/images/workspacePage5.png) 

–  Click Record to launch the browser. While recording, actions performed on the browser will be captured and generated into test steps. Provide start url and device, click OK of Record dialog when you start recording.

![](/assets/images/record1.png) 

–  Let's create a simple script by going to Google Search and searching for some keywords as illustrated on the screen above. 

![](/assets/images/record2.png) 

![](/assets/images/record4.png) 

–  Click the stop button from the main Toolbar to stop recording, captured actions and objects are generated in last-hit.

![](/assets/images/record5.png) 

–  Now you can click on replay command from the main Toolbar to execute the script.
![](/assets/images/replay1.png) 

–  Click ok to start replay.

![](/assets/images/replay3.png)

![](/assets/images/replay2.png) 

Congratulations! You have just successfully created and executed your first test case.

For further instructions and help, please refer to last-hit User Guide or last-hit Forum.

## Resources for Learning last-hit

- [last-hit.org/docs](https://last-hit.org/docs) - all of last-hit's documentation
- [electronjs.org/docs](https://electronjs.org/docs) - all of Electron's documentation
- [puppeteer/docs](https://github.com/GoogleChrome/puppeteer/tree/master/docs) - all of Puppeteer's documentation


## License

[Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/)
