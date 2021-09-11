# visitor-logging-course



# Skill Overview

\&lt;!-- ( **start** ) Source:[https://www.ibm.com/developerworks/security/library/se-bluemix-self-posting-app-mean-stack-part1/index.html?ca=drs-](https://www.ibm.com/developerworks/security/library/se-bluemix-self-posting-app-mean-stack-part1/index.html?ca=drs-)and edited by Abdullah Tasleem --\&gt;

In this skill, you will learn how to use the IBM Cloud to write a Node.js application for an organization&#39;s front desk, which needs to log visitors in and out. Along the way you will learn how to use **HTML** , **JavaScript** , **Node.js** , the **Express** HTTP server library, and a **Cloudant** database. You will learn how to do this in the highly available IBM Cloud using an online **Eclipse Orion** IDE. This is a basic introduction to back-end programming on the IBM Cloud platform.

### Objectives

**By the end of this skill, you should be able to:**

- Create and deploy Node.js apps using an online IDE
- Understand and use basic Express commands
- Make basic function calls using JavaScript
- Create a basic UI using HTML &amp; JavaScript
- Make sense out of JSON files
- Create test functions for your web application
- Store and retrieve data from a database

### Prerequisites

It is recommended to have some basic coding knowledge for this skill. In order to be familiar with **Node.js** &amp; **HTML** and understand the steps taken in the exercise, it is recommended to complete [Create your own web page](https://developer.ibm.com/digitalnation/africa/course/innovator-create-your-own-web-page/?lang=en&amp;course-lang=en) course.

In this skill, you will learn how to use the IBM Cloud to write a Node.js application for an organization&#39;s front desk, which needs to log visitors in and out. Along the way you will learn how to use **HTML** , **JavaScript** , **Node.js** , the **Express** HTTP server library, and a **Cloudant** database. You will learn how to do this in the highly available IBM Cloud using an online **Eclipse Orion** IDE. This is a basic introduction to back-end programming on the IBM Cloud platform.

### Objectives

**By the end of this skill, you should be able to:**

- Create and deploy Node.jsJS apps using an online IDE
- Understand and use basic Express commands
- Make basic function calls using JavaScript
- Create a basic UI using HTML &amp; JavaScript
- Make sense out of JSON files
- Create test functions for your web application
- Store and retrieve data from a database

### Prerequisites

It is recommended to have some basic coding knowledge for this skill. In order to be familiar with **Node.js** &amp; **HTML** and understand the steps taken in the exercise, it is recommended to complete [Create your own first professional web page](https://developer.ibm.com/africa/skills/innovator-create-your-first-professional-web-page-using-html-css/)course.

# Getting Started with Back-End

## Introduction to JavaScript

You were given a quick introduction to JavaScript in the first course. Since we will be using it a lot more here, let&#39;s have a quick overview about the basic elements of JavaScript.

### Variables

_Variables_ are containers for storing data values that can later be retrieved or updated with new data. The data stored in a variable can be a _value_ or _expression_. There are three types of expressions in the JavaScript language:

- **ArithmeticNumerical:** Evaluates to a number. Example: 10 or 99
- **String:** Evaluates to a string. Example: &quot;John&quot; or &quot;home&quot;
- **Logical:** Evaluates to a Boolean (true or false). Example: true or false, yes or no.

Variables in JavaScript are declared with the var keyword. With the var keyword, the variable is considered _local_ because it cannot be accessed anywhere outside the scope of the place that you declared it.

You have several options on structuring your variable declaration and initialization:

|
 |
 |
| --- | --- |
| // declaring one variable |

|
 |
 |
| --- | --- |
| varcost; |

|
 |
 |
| --- | --- |
|                  |

|
 |
 |
| --- | --- |
| // declaring multiple variables, delimited by commas |

|
 |
 |
| --- | --- |
| varcost, profit;   |

|
 |
 |
| --- | --- |
|            |

|
 |
 |
| --- | --- |
| // declaring and assigning one variable |

|
 |
 |
| --- | --- |
| varcost = 120;   |

|
 |
 |
| --- | --- |
|              |

|
 |
 |
| --- | --- |
| // declaring and assigning multiple variables |

|
 |
 |
| --- | --- |
| varcost = 120, profit = 77; |

If a variable is not declared explicitly (using var), then JavaScript will automatically treat it as a _global_ variable. Global variables are accessible throughout the entire script.

### Functions

A JavaScript function is a block of code designed to perform a particular task. A function is executed when &quot;something&quot; invokes it (calls it).it is invoked/called within the code.

Functions are useful for many reasons. They are containers for contain the script code that runs only by an event or a call to the function. Therefore, functions do not execute when the browser initially loads and executes the script that is included in the web page.

A function contains the script that has a specific task so you can execute that script and run that task any time.

An example of how a function looks like in JavaScript and how to call it is given below:

|
 |
 |
| --- | --- |
| varnum = 10; |

|
 |
 |
| --- | --- |
|   |

|
 |
 |
| --- | --- |
| functionchangeVariableValue() |

|
 |
 |
| --- | --- |
| { |

|
 |
 |
| --- | --- |
|    num = 11; |

|
 |
 |
| --- | --- |
| } |

|
 |
 |
| --- | --- |
| changeVariableValue(); |

|
 |
| --- |

console.log(&quot;num is: &quot;+ num);

To learn more about JavaScript you can take the [JavaScript Course](https://developer.ibm.com/africa/skills/javascript/) in [New Collar section of the website](https://developer.ibm.com/africa/new-collar/).New collar

## Introduction to Express

The default Node.js framework provides a limited set of features for building web applications. Therefore, developers rely on third-party packages to extend the Node&#39;s Node.js features.

The **Express** web application framework is one of the most popular building blocks for web applications.

**Express** is a Node.js web framework. It allows rapid development of web applications. It also provides an easy way to manage application routing by making REST APIs available.

**Express** is a third-party module that provides a framework for building web applications. It implements an &quot;app&quot; class that you can map to a web resource path.

We will be using **Express** extensively in this course, if you would like to learn more about about Express you can take the [Express Web Framework](https://developer.ibm.com/africa/skills/express-web-framework/) course in the [New collarCollar section of the website](https://developer.ibm.com/africa/new-collar/).

## Introduction to Databases and JSON

_Databases_ are applications that allow you to store and access data. Web applications use them to provide dynamic functions to users, such as displaying products, content management, and user management.

Different types of databases are available. Generally, they are divided in to **relational** ( **SQL** ) databases and **non-relational** ( **NoSQL** ) databases. **Relational Database Management System (RDBMS)** is a common type of database in which data is stored according to the relationship it has to other data. In many implementations, an **RDBMS** consists of storingstores data in different tables and building relationships between rows in the tables. **NoSQL** ( **Not only SQL** ) on the other hand is a database which is created in means other than a tabular format. It&#39;s an alternative to the **RDBMS** where data is carefully placed in tables and data schemas.

In this course we will be using a cloud database called **Cloudant** which is a **NoSQL** database.

Acloud database is a database service built and accessed through a cloud platform. It serves many of the same functions as a traditional database with the added flexibility of cloud computing. Users install software on a cloud infrastructure to implement the database.

Key features:

- A database service built and accessed through a cloud platform
- Enables enterprise users to host databases without buying dedicated hardware
- Can be managed by the user or offered as a service and managed by a provider
- Can support SQL (including MySQL) or NoSQLSupport both relational and non-relational databases
- Accessed through a web interface or vendor-provided API

To learn more about **cloudant Cloudant** you can visit [this link](https://www.ibm.com/cloud/learn/what-is-cloud-database).

# Exercise: Create a front-desk visitor logging tracking app

## Objectives

This exercise will teach you how to setup your online development environment and then use it to code and deploy applications on IBM Cloud. We will create Node.js application for an organization&#39;s front desk using multiple tools and services. We will explain all the steps and anything new that you will encounter along the way. It&#39;s important to note that in this exercise we have large blocks of code, so first we ask you to copy that code and then after that we explain it line by line.

You need an active [IBM Cloud](https://console.bluemix.net/) Lite account (provided with your D-NA account) to proceed.

**Estimated time to complete this exercise:** 150 minutes

**_Exercise Summary Steps_**

In this exercise, you will:

- Create and deploy a sample application
- Set up your working environment
- Create the back-end application for Visitor Log
- Create a basic UI of the app
- Create and use a Cloud Database

## Create the application

1. Log in to the [IBM Cloud](https://cloud.ibm.com/). Click on the hamburger menu icon on the top left. ![image001](https://user-images.githubusercontent.com/27959350/132950668-66ea2cad-eeb8-40dc-9396-7bdbc2a9cca0.jpg)

 Figure 1. IBM Cloud Dashboard
2. Select **Cloud Foundry** -\&gt; **Public**. <img width="502" alt="image002" src="https://user-images.githubusercontent.com/27959350/132950669-6250a4ba-eda0-4c43-b0f6-3fb7e81cc8cf.png">

 Figure 2. Hamburger menu

3. Click **Create** on the top right. ![image003](https://user-images.githubusercontent.com/27959350/132950670-cb69ab58-9ba0-4e2a-ae98-8e124bee257d.png)

 Figure 3. Cloud Foundry menu

4. Make sure the following is selected and then click **Create** :

| **Region/location** | Choose **London** if available or else whichever is closest to you (which ever one you usually use with your lite account) |
| --- | --- |
| **Pricing Plan** | Select 64 MB |
| **Resource** | Select the **SDK for Node.js** |
| **App Name** | Give it any name of your choosing but it has to be unique. If you wish to go with the name similar to the screenshot then change the number &quot;100&quot; to any other unique number of your choosing |
| **Domain** | You can leave this as default |
| **Organization and space** | Leave the default (if you don&#39;t see any then make sure you have the right region selected) |

![image004](https://user-images.githubusercontent.com/27959350/132950672-01fdc5f7-0783-4182-a761-72fab8f00dcc.png)


 Figure 4. Setting up a Cloud Foundry application ![image005](https://user-images.githubusercontent.com/27959350/132950673-675ad739-d64c-4e6b-bb66-83b88012561a.png)

 Figure 5. Setting up a Cloud Foundry application (2)

1. Wait for the application to start, you will see a rotating starting bar. <img width="964" alt="image006" src="https://user-images.githubusercontent.com/27959350/132950674-67a4b1ee-bf23-478c-9ea1-f367da17bb3f.png">
Figure 6. Cloud Foundry application is starting up

2. Once the app is running, go ahead and click **Visit App URL**. <img width="677" alt="image007" src="https://user-images.githubusercontent.com/27959350/132950675-e5c430f4-b43a-4f9f-a3b4-fe2e4f3aab8c.png">

 Figure 7. Deployed Cloud Foundry application

3. Now you should see the initial application. After you see it, do not close the tab. You will need it later. ![image008](https://user-images.githubusercontent.com/27959350/132950676-44190631-1ec8-442e-8e59-5da909a9e1fb.png)

 Figure 8. Hello World Screen

1. Log on in to the [IBM Cloud ConsoleIBM Cloud](https://console.bluemix.net/).
2. Expand the hamburger icon on the top left and select **Cloud Foundry**.

<img width="635" alt="image009" src="https://user-images.githubusercontent.com/27959350/132950677-83ec6d0b-91ca-4c78-8386-07fe8a393ede.png">


Figure 1. IBM Cloud Dashboard

<img width="161" alt="image010" src="https://user-images.githubusercontent.com/27959350/132950678-2e0a5c52-2e4d-4d24-b9dc-416d9e2b63f3.png">


Figure 2. Hamburger menu

1. Hover over the **Public Applications** section and click **Create.**

<img width="514" alt="image011" src="https://user-images.githubusercontent.com/27959350/132950679-1a4748e9-7a80-4fda-93f3-75445fd81595.png">


Figure 3. _Clou_d Foundry menu

1. Select the **SDK for Node.js**

 ![](RackMultipart20210911-4-8gav30_html_66c47b09de7b1256.png)

Figure 4. Cloud Foundry applications

1. Enter the following and then click **Create** :

| **App name** | Pick any unused name |
| --- | --- |
| **Host name** | Accept the default name that will appear once you enter the app name |
| **Domain** | eu-gb.mybluemix.net |
| **Region/location** | Choose **United Kingdom** if available or else whichever is closest to you |
| **Organization and space** | Leave the default |

![](RackMultipart20210911-4-8gav30_html_10a66ecb0809675a.png)

Figure 5. Setting up a Cloud Foundry application

1. Wait for the application to start, you will see a rotating starting bar.

 ![](RackMultipart20210911-4-8gav30_html_55d2200dd16278d1.png)

Figure 6. Cloud Foundry application is starting up

1. Once the app is awake (running), go ahead and click **Visit App URL**.

 ![](RackMultipart20210911-4-8gav30_html_166e8a1b7768f987.png)

Figure 7. Deployed Cloud Foundry application

1. Now you should see the initial application. After you see it, do not close the tab. You will need it later.

![](RackMultipart20210911-4-8gav30_html_30cc7695d567f227.png)

Figure 8. Initial application&#39;s screen

## Create the development environment

Cloud Foundry on the IBM Cloud allows several development environments. In the last course we used Command Line to deploy our Node.js application. In this course, we will take the easier approach where you don&#39;t have to install anything on your local machine and use the online development environment.

1. Return to the IBM Cloud page by clicking on **IBM Cloud** on the top left. Click on the **Cloud Foundry apps** under resources in the dashboard. ![](RackMultipart20210911-4-8gav30_html_b7558750b9ec1bbd.png)
 Figure 1. IBM Cloud Dashboard - Resources
2. Open your application by clicking on its name as shown in the figure below: ![](RackMultipart20210911-4-8gav30_html_51459ce500b58a78.png)
 Figure 2. Cloud Foundry App

3. Scroll down to **Continuous Delivery** and click **Enable Continuous Delivery**. ![](RackMultipart20210911-4-8gav30_html_6e869d624847ea08.png) Figure 3. Continuous Delivery

4. All the fields should already be filled out. You just need to go to the **Delivery Pipeline** to create an API key.
 ![](RackMultipart20210911-4-8gav30_html_852174660bc60908.png)
 Figure 4. Setting up continuous delivery

5. Create an **IBM Cloud API Key**. You can do that by clicking the **New +** button shown in the figure below. ![](RackMultipart20210911-4-8gav30_html_51cfeace7074b3ee.png) Figure 5. Setting up continuous delivery (2)
6. It will ask for a confirmation, click on **OK**. ![](RackMultipart20210911-4-8gav30_html_39db571618d06274.png) Figure 6. Setting up continuous delivery (3)

7. Once the API Key appears you can go ahead and **Create** the toolchain. ![](RackMultipart20210911-4-8gav30_html_74460725a77c595e.png) Figure 7. Setting up continuous delivery (4)
8. You should now have the toolchain created. Go ahead and click on **Eclipse Orion Web IDE** to start coding your application. ![](RackMultipart20210911-4-8gav30_html_5870e51e6ec20792.png)
 Figure 8. Toolchain

9. Once you are on your coding environment, click on **Create new launch configuration \&gt; +**.
 ![](RackMultipart20210911-4-8gav30_html_3c25abe49788f111.png)
 Figure 9. Eclipse Orion Web IDE

10. In the **Edit Launch Configuration** , it will try to load the deployment settings for you. But it might set the **Target** as Dallas or Germany by default, so you need to make sure it has your region selected. Since we selected our region as London earlier, go ahead and choose London in the **Target** field. ![](RackMultipart20210911-4-8gav30_html_2c0c6e3bf6a09a5a.png)
 Figure 10. Deployment settings editor

11. Once you choose your region as the target region it will load the deployment settings for you (if it doesn&#39;t then you don&#39;t have the right region selected). Just double check all the fields if everything is ok and then click on **Save**.
 ![](RackMultipart20210911-4-8gav30_html_e0b37a609faa45d6.png)
 Figure 11. Editing deployment settings
12. Now let&#39;s move on to the **app.js** file on the left navigation menu. This is the main Node.js application code file. The **index.html** file is the main **view** file and **app.js** is the main **back-end** file in such applications. ![](RackMultipart20210911-4-8gav30_html_ddfb0001648bfbbd.png)
 Figure 12. Application&#39;s files

13. Add the following lines of code just before the definition of variable appEnv:
14. app.get(&quot;/hello&quot;,/\* @callback \*/function(req, res){
15. res.send(&quot;Hello, world&quot;);

});

1. The code will look like the one in the figure below. ![](RackMultipart20210911-4-8gav30_html_d8761691d19869ba.png) Figure 13. Code editor
2. Once you have added the code, you can go ahead and click on the play button at the top (as shown below) to apply the changes. ![](RackMultipart20210911-4-8gav30_html_56b483410041fa36.png)
 Figure 14. Deploying application

3. It will ask for a confirmation to stop and redeploy the app, click on **OK**. ![](RackMultipart20210911-4-8gav30_html_c109af623261c96.png) Figure 15. Confirmation for deploying application

4. The application will start deploying and you will see the loading screen as shown below.
 ![](RackMultipart20210911-4-8gav30_html_f19e8130a9ce244e.png)
 Figure 16. App being deployed

5. Wait until you see the green circle again and bracket says running: normal (might take a few minutes). This means that the application was restarted with the new code successfully. ![](RackMultipart20210911-4-8gav30_html_9a5544d7282dc0c8.png)
 Figure 17. Application is deployed

6. Once ready, open the deployed application by clicking on the button shown below: ![](RackMultipart20210911-4-8gav30_html_6f5f84999187e1b2.png)
 Figure 18. Open Application
7. The application will open and you will see the normal hello world screen for now. ![](RackMultipart20210911-4-8gav30_html_d3e611d140086be7.png)
 Figure 19. Main page

8. Now to make your new lines of code work, add /hello at the end of your app URL as shown below. See that you get a &quot;Hello, world&quot; message reply on a plain screen. ![](RackMultipart20210911-4-8gav30_html_90449fe02c6f6df6.png) Figure 20. &quot;Hello, world&quot; page

Great! You have successfully set up your deployment environment and deployed your **Hello World** program using an online IDE.

Now let&#39;s try to understand the source code we just played around with in the **app.js** file.

The first line is ignored by the JavaScript interpreter since it is a comment. A comment in programming is a readable explanation or annotation for whoever is looking at the code. Its purpose is usually to make the code easier to understand or to make the compilers and interpreters ignore certain sections of code.

This particular comment is here to inform you that the IBM Console editor includes the Eslint utility to identify potential errors in the code. This directive tells that utility to treat the JavaScript as Node.js (server-side JavaScript) code. [You can read more about the Eslint utility here](https://eslint.org/docs/user-guide/configuring).

/\*Eslint-env node\*/

In JavaScript comments are denoted either by using the /\* \*/ tags to ignore a block of the code or by typing a double slash (//) at the beginning of the line to ignore that line:

//------------------------------------------------------------------------------

// node.js starter application for Bluemix

//------------------------------------------------------------------------------

**Node.js** is the runtime environment. The web server package is **Express**. **Express** is a web application framework to provide a back-end and a way to manage it for the **Node.js** application.[You can read more about it here](http://expressjs.com/). The way you use a package in Node.js is to use the require() function with the package name (assuming the package is declared in the **package.json** file). The require() function usually returns a specified module.

// This application uses express as its web server

// for more info, see: http://expressjs.com

var express =require(&#39;express&#39;);

The cfenv module provides Cloud Foundry information. It is used later to get the port number to which the web server needs to listen, and the URL it is serving.

// cfenv provides access to your Cloud Foundry environment

// for more info, see: https://www.npmjs.com/package/cfenv

var cfenv =require(&#39;cfenv&#39;);

The next step is to create a **Hypertext Transfer Protocol** ( **HTTP** ) server. **HTTP** is the protocol used by **World Wide Web** ( **WWW** ) that defines how messages are exchanged within the **WWW** and how to respond to these messages. If you load a URL online, the web page is loaded up after an **HTTP** command is sent to the web server to get the page.

// create a new express server

var app =express();

This is how we tell Express to serve static files from a directory. If you open the public directory in the editor, you will see the index.html file that is part of the default application.

// serve the files out of ./public as our main files

app.use(express.static(\_\_dirname +&#39;/public&#39;));

The app.get call specifies how to handle requests for a particular path. The call has two parameters – a parameter is a variable that is used to pass information between functions. The path (&quot;/hello&quot;) is the first parameter and the second parameter is an anonymous function to call when the path is requested. So this basically means that whenever the app sees the word &quot;hello&quot; in its URL path, it will call this anonymous function (function with no name that is defined at runtime). This function has two further parameters: a request object that includes the HTTP request, and a response object used to send back a response (in our case it responds with the text &quot;Hello, world&quot;).

The callback function just uses the res.send function to send a constant string, the traditional &quot;Hello, world&quot;.

The /\* @callback \*/ comment is for **Eslint**. Normally, **Eslint** would report that a function has an unused parameter and suggest you remove it. However, the parameters of callback functions are set by the calling code (here, Express). In this case, some path callbacks require both parameters.

app.get(&quot;/hello&quot;,/\* @callback \*/function(req, res){

res.send(&quot;Hello, world&quot;);

});

The variable appEnv gets the Cloud Foundry environment. This is how the IBM Cloud infrastructure communicates with the application. [You can read more about this here](https://www.npmjs.com/package/cfenv).

// get the app environment from Cloud Foundry

var appEnv = cfenv.getAppEnv();

// start server on the specified port and binding host

app.listen(appEnv.port,&#39;0.0.0.0&#39;,function(){

// print a message when the server starts listening

console.log(&quot;server starting on &quot;+ appEnv.url);

});

Cloud Foundry on the IBM Cloud allows several development environments. In the last course we used Command Line to deploy our nodeNode.js application. In this skill, we take the other easier road approach where you don&#39;t have to install anything on your local machine and use the web online development environment.

1. Return to the IBM Console Cloud page for the application. If you are logged out, log back in and click the application&#39;s name in the dashboard as shown below:

 ![](RackMultipart20210911-4-8gav30_html_1a5ff8b6daed1998.png)

Figure 9. IBM Cloud Dashboard (with the Cloud Foundry application present)

1. Scroll down to continuous delivery and click **Enable**.
2.


 ![](RackMultipart20210911-4-8gav30_html_28bb8aaa81ea243a.png)

Figure 10. Application&#39;s dashboard

1. All the fields should already be filled out. All you only need to do is go to the **Delivery Pipeline** and create an **IBM Cloud API Key**. You can fo do that by clicking on the **Create** button shown in the figure below.

 ![](RackMultipart20210911-4-8gav30_html_888f67708d442a08.png)

Figure 11. Setting up continuous delivery

1. Once the API Key appears you can go ahead and create the toolchain.

 ![](RackMultipart20210911-4-8gav30_html_6c5cf0347f58944d.png)

Figure 12. Setting up continuous delivery

1. You should now have the toolchain created. Click on **Eclipse Orion Web IDE** to start coding your application.

 ![](RackMultipart20210911-4-8gav30_html_3e74ea5d0d63846e.png)

Figure 13. Setting up continuous delivery

1. Click **Create new launch configuration** \&gt; **+**.
2.

 ![](RackMultipart20210911-4-8gav30_html_5dc5a9e9effcb573.png)

Figure 14. Eclipse Orion Web IDE

1. In the **Edit Launch Configuration,** it will try to load the deployment settings for you. But it might set the **Target** as Germany by default, so you need to make sure it has your region selected. Since we selected our region as UK earlier, go ahead and choose United Kingdom in the **Target** field.

 ![](RackMultipart20210911-4-8gav30_html_984afab779e300a2.png)

Figure 15. Deployment settings editor

1. Once you choose your region as the target it will load the deployment settings for you. Just double check all the fields if everything is ok click on **Save**.

 ![](RackMultipart20210911-4-8gav30_html_ca9bc775d2a82228.png)

Figure 16. Editing deployment settings

1. Now let&#39;s move on to the **app.js** file on the left navigation menu. This is the main Node.js file where we will code the application code file in. The **index.html** file is the main **viewing** file and **app.js** is the main **back-end** file in such applications.

 ![](RackMultipart20210911-4-8gav30_html_5d5cdb4059544b11.png)

Figure 17. Application&#39;s files

1. Add the following lines of code just before the definition of variable appEnv:


app.get(&quot;/hello&quot;, /\* @callback \*/ function(req, res) {

res.send(&quot;Hello, world&quot;);

});

 The code will look like the one in the figure below.

 ![](RackMultipart20210911-4-8gav30_html_27601fb3c40eedc0.png)

Figure 18. Code editor

Once you add it you can go ahead and click on the play button at the top (as shown above) to apply the changes.

1. The application will start deploying and you will see the screen below.

 ![](RackMultipart20210911-4-8gav30_html_7c7f5e1619dda9e.png)

Figure 19. Deploying application

1. Wait until you see the green circle again. It means that the application was restarted with the new code.

 ![](RackMultipart20210911-4-8gav30_html_77c36121b60cbac5.png)

Figure 20. Application is deployed

1. Go back to the application tab and add /hello at the end of the URL. See that you get a &quot;Hello, world&quot; message as shown below:

 ![](RackMultipart20210911-4-8gav30_html_fce07b1d4ca81054.png)

_Figure 21. &quot;Hello, world&quot; page_

Great! You have successfully set up your deployment environment and deployed your **hello Hello world World** program using an online IDE.

 Now let&#39;s try to understand the source code we just played around with in the **app.js** file

 The first line is ignored by the JavaScript interpreter since it is a comment. A comment in programming is a readable explanation or annotation for whoever is looking at the code. Their Its purpose is usually to make the code easier to understand or just addedto make for the compilers and interpreters to ignore certain sections of code.

It isThis particular comment is here because to inform you that the IBM Console editor includes the **Eslint** utility to identify potential errors in the code. This directive tells that utility to treat the JavaScript as Node.js (server-side JavaScript) code. [You can read more about the Eslint utility here](https://eslint.org/docs/user-guide/configuring).

/\*Eslint-env node\*/

In JavaScript comments are denoted either by using the /\* \*/ ttags to ignore a block of the code or the other way isby to typinge in a double slash (//) at the beginning of the line to ignore that linethrough which the rest of the line after it is ignored as a comment:

//------------------------------------------------------------------------------

// node.js starter application for Bluemix

//------------------------------------------------------------------------------

**Node.js** is the runtime environment. The web server package is **Express**. **Express** is a web application framework to provide a back-end and a way to manage it for the **Node.js** application. [You can read more about it here](http://expressjs.com/). The way you use a package in Node.js is to use the require() function with the package name (assuming the package is declared in the **package.json** file). The require() function usually returns a function that you use to use thespecified module.

// This application uses express as its web server

// for more info, see: http://expressjs.com

var express = require(&#39;express&#39;);

The cfenv module provides Cloudy Foundry information. It is used later to get the port number to which the web server needs to listen, and the URL it is serving.

// cfenv provides access to your Cloud Foundry environment

// for more info, see: https://www.npmjs.com/package/cfenv

var cfenv = require(&#39;cfenv&#39;);

The next step is to create a **Hypertext Transfer Protocol** ( **HTTP** ) server. **HTTP** is the protocol used by **world World wide Wide web Web** ( **WWW** ) that defines how messages are exchanged within the **WWW** and how to respond to these messages. If you load a URL online, the web page is loaded up after an **HTTP** command is sent to the web server to get the page.

// create a new express server

var app = express();

This is how we tell **Express** to serve static files from a directory. If you open the **public** directory in the editor, you will see the **index.html** file that is part of the default application.

// serve the files out of ./public as our main files

app.use(express.static(\_\_dirname + &#39;/public&#39;));

The app.get call specifies how to handle requests for a particular path. The call has two parameters – a parameter is a variable that is used to pass information between functions. The path (&quot;/hello&quot;) is the first parameter and the second parameter is an anonymous function to call when the path is requested. So this basically means that whenever the app sees the word &quot;hello&quot; in its URL path, it will call this anonymous function (function with no name that is defined at runtime). This function has two further parameters: a request object that includes the HTTP request, and a response object used to send back a response (in our case is responds with the text &quot;Hello, world&quot;).

The callback function just uses the res.send function to send a constant string, the traditional &quot;Hello, world&quot;hello world.

The /\* @callback \*/ comment is for **Eslint**. Normally, **Eslint** would report that a function has an unused parameter and suggest you remove it. However, the parameters of callback functions are set by the calling code (here, Express). In this case, some path callbacks require both parameters.

app.get(&quot;/hello&quot;, /\* @callback \*/ function(req, res) {

    res.send(&quot;Hello, world&quot;);

});

The variable appEnv gets the Cloud Foundry environment. This is how the IBM Cloud infrastructure communicates with the application. [You can read more about this here](https://www.npmjs.com/package/cfenv).

// get the app environment from Cloud Foundry

var appEnv = cfenv.getAppEnv();

// start server on the specified port and binding host

app.listen(appEnv.port, &#39;0.0.0.0&#39;, function() {

  // print a message when the server starts listening

  console.log(&quot;server starting on &quot; + appEnv.url);

});

## The Visitor Log


The main data structure of the application is a visitor log. Let&#39;s try it out and see how it looks.

1. You can get the source code that declares and manipulates the visitor log [by going to this github link](https://github.com/qbzzt/bluemix/blob/master/security/201803/Visitor_Log/02-app.js). Click on the **raw** button to easily copy the entire code. ![](RackMultipart20210911-4-8gav30_html_f9f804757afd147.png) Figure 1. Github page
2. Copy all the code in that file. ![](RackMultipart20210911-4-8gav30_html_7d5d9352c2695d8d.png) Figure 2. Copy code
3. Replace the code in your current **app.js** file with the one you just copied and then press the **play** button to restart the application (make sure you completely remove all the code from the **app.js** file before pasting your code). ![](RackMultipart20210911-4-8gav30_html_8824e17094b3fc15.png) Figure 3. Replacing current code
4. Once again, the IDE might ask you for a confirmation to stop and redeploy, proceed with it. ![](RackMultipart20210911-4-8gav30_html_2f7c3ef2d024aa5d.png) Figure 4. Confirmation box
5. Open the deployed app again by clicking on the button shown below: ![](RackMultipart20210911-4-8gav30_html_879d143dbac71c59.png) Figure 5. Open deployed app

6. You can see the current visitor log by adding the text: **test/visitors** at the end of your application URL. It will look like this: ![](RackMultipart20210911-4-8gav30_html_46b327356659c05e.png) Figure 6. Visitor log The text you see on the page is called **JavaScript Object Notation** ( **JSON** ). Some browsers format it as shown above, however, sometimes the output might look like this raw data: ![](RackMultipart20210911-4-8gav30_html_ef7a7145e00cf653.png) Figure 7. Unformatted JSON opened in a browser You can make it more readable by using [a JSON formatter such as this one](https://jsonformatter.curiousconcept.com/). Just copy and paste the raw data that you will get (like the one in the figure above) into this link and it will be formatted to something you can understand. It will look like this: ![](RackMultipart20210911-4-8gav30_html_333b22858fbb2113.png)
 Figure 8. Expanded JSON If you are interested to see the visitor log for our sample application instance, [click here](https://visitor-log-qbzzt.mybluemix.net/test/visitors?cm_mc_uid=62379037222015373600237&amp;cm_mc_sid_50200000=26941741538569905159&amp;cm_mc_sid_52640000=72791401538569905167).

7. Let&#39;s try to understand what this visitor log json object is telling us. This visitor log is an **associative array** (also called a **hash table** , or an **object** ). Associative arrays have **key-value** pairs. Instead of storing data in a linear way like with the normal arrays (array[0]=&quot;Bill Hamm&quot;), here you store the data as a **collection** and assign it one unique value. You can later call these values from anywhere using a particular syntax. The associative array here has **keys** which are visitor names (for example: &quot;Bill Hamm&quot;). The **value** for each of these keys (visitor names) is itself another associative array, which can have two **attributes** ( **keys** ):
arrived - The last time the visitor arrived at the office. This attribute does not exist if the visitor is not currently in the office.
history - The visitor&#39;s history, an array of associate arrays with the start and end times of previous visits. This attribute does not exist during the first visit to the office.

8. As you can see in the previous figures that we already have some sample data for testing purposes. This data was defined in the code that we used earlier, here is the code snippet:
9. // Visitors data structure
10. var visitors ={
11. &quot;Bill Hamm&quot;:{
12. arrived:newDate(Date.now()-1000\*3600\*2)
13. },
14. &quot;Deborah Lapidot&quot;:{
15. arrived:newDate(Date.now()-1000\*3600),
16. history:[
17. {
18. arrived:newDate(Date.now()-26\*1000\*3600),
19. left:newDate(Date.now()-24\*1000\*3600)
20. }
21. ]
22. },
23. &quot;Ehud ben-Gera&quot;:{
24. history:[
25. {
26. arrived:newDate(Date.now()-(3\*24+3)\*1000\*3600),
27. left:newDate(Date.now()-(3\*24-1)\*1000\*3600)
28. },
29. {
30. arrived:newDate(Date.now()-(2\*24+2)\*1000\*3600),
31. left:newDate(Date.now()-(2\*24-5)\*1000\*3600)
32. }
33. ]
34. }

};

You can also find this code snippet in your IDE here:

![](RackMultipart20210911-4-8gav30_html_cc81de0cdefa6624.png) Figure 9.Code Snippet Most of it is a standard JavaScript object definition, but the dates, instead of being constants, are now assigned to a short amount of time before the application&#39;s start. Date.now() is the number of milliseconds between now and a fixed point in time (midnight January 1st 1970 GMT). So Bill Hamm&#39;s arrival time is two hours before this code is executed when the application starts. [You can read more about the Date object here](https://www.w3schools.com/jsref/jsref_obj_date.asp).

&quot;Bill Hamm&quot;:{

arrived:newDate(Date.now()-1000\*3600\*2)

},

### Reading the visitor log

When displaying the visitor log, we might want to display all of it, or we might want to display just the current visitors, those that are currently in the office. Also, it can be useful to get the names of all the visitors, all the visitors currently in the office, or all those who currently aren&#39;t, without their full information. These are the functions that implement these requirements:

1. To get the list of visitor names, all we need is to get the keys of the visitors object. The function to do this is Object.keys. Note that the function syntax here is the new one:
2. varFunction\_Name=(Parameter\_1, Parameter\_2, …, Parameter\_N)=\&gt;
3. {
4. \&lt;\&lt;Function code goes here\&gt;\&gt;

}

  To get a subset (either those who are in the office or those who aren&#39;t), use the filter() function. It returns an array of elements that pass a particular test. It gets one parameter, a function. This function gets an item from the list as a parameter and returns whether or not that item should be a member of the filtered list. In our case we are trying to filter out all the visitor names that have arrived in the office (in coding: those whose arrived values are not equal to undefined). This function is an array method (so you can call it on any list, such as the one returned by visitorNames).
 When a function literal is a single expression, there is no need to enclose it in curly brackets ({}) and have a return statement. You can just enter the expression.

varcurrentVisitorNames=()=\&gt;{

returnvisitorNames().filter((name)=\&gt; visitors[name].arrived !==undefined);

};

 By using the filter() function we just got the list of names who have arrived in the office but not their details that were there in the default visitor log. It is a bit more complicated to get the list of current visitors with their information, with the names as keys.

 Then next step is to create list with of currently present visitors called currentVisitorList. This function uses the map() function to retrieve the information for each user in the list of current visitors. This function receives a function as a parameter, similar to filter() function. However, instead of deciding whether a value will be in the output or not, the function in map is used to transform the values:

- It creates a new array
- This array is populated with the mapping function results
- Every time the mapping function is executed, it receives the data of the currently present visitor and puts it an object
- Afterwards, these objects are put in a list in the same order as the original values

[You can learn more about this function here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map). In this case, for each name we get a structure with the user information. For example, if you add /test/currentVisitorList at the end of your application URL, you will get the list of current visitors with their information that we got using the mapping function.

varcurrentVisitorList=()=\&gt;{

returncurrentVisitorNames().map((name)=\&gt;{

var retVal ={};

retVal[name]= visitors[name];

return retVal;

});

};

 ![](RackMultipart20210911-4-8gav30_html_20cb492f2f2ab155.png)
 Figure 10. currentVisitorList This list has the information we need. However each user is in a separate object. It makes a lot more sense to use the same format we use in the visitors variable, one object with each user being a separate attribute.

 The final step is to turn the list of current visitors in a single object. To achieve that, we use the reduce() function. If the list it receives has one item, it returns that item. If it has two items, it runs the parameter function on them and returns the result. If there are more, it runs the parameter function on two of them, then on that result and another one, until there is only a single value left. [You can read more about the function here](https://www.w3schools.com/jsref/jsref_reduce.asp).

varcurrentVisitors=()=\&gt;{

returncurrentVisitorList().reduce((a, b)=\&gt;{

var bKey = Object.keys(b)[0];

a[bKey]= b[bKey];

return a;

});

};

1. To create the combined object, we first need the key of the new object, the one from the list which only has a single attribute for a single user (var bKey = Object.keys(b)[0];).
 We add this value to the original object, the one in which we accumulate all the users (a[bKey] = b[bKey];). Then we finally return it.

### Updating the visitor log

There are two ways to make modifications to the visitor log. A user may be logged in when they enter the office or logged out when they leave.

For these functions we have a **get** function and a **set** function to interact with the visitors variable. The get function gets the details of a visitor when it is given a name and the set function sets a new visitor or updates existing details of a visitor when given a name and its value. The purpose of these functions is to make it easy to modify the application to use a different data storage, for example a database, in the future.

vargetVisitor=(name)=\&gt; visitors[name];

varsetVisitor=(name, values)=\&gt; visitors[name]= values;

Let us look at the logout() function now by breaking it down line by line:

1. The log out function is relatively simple. First, we store the details of that particular visitor in a new variable oldRecord.
2. varlogOut=(name)=\&gt;{

var oldRecord =getVisitor(name);

  Then we check if the visitor even exists, if the name is not found, then we return text saying that there is an error.

if(oldRecord ===undefined)

return`Error, ${name} is unknown`;

  Next, we check whether the user has an arrived attribute. If the user doesn&#39;t have it, this user is not currently in the office and cannot be logged out. Report an error.

if(oldRecord.arrived ===undefined)

return`Error, ${name} is not logged in`;

  If there is no error till now it means the visitor is in the system and is logged in. Then the only attribute in the old record that is still relevant is history. We need to keep it and add a new value to it. However, if this is the first visit there might be no history yet. In such a case, the history is empty.

var history = oldRecord.history;

// If this is the first visit

if(history ===undefined)

history =[];

  The unshift function adds a new value at the beginning of an array. This is the behavior we want here, because the latest visits are more likely to be relevant, so it is best if the array is sorted in reverse chronological order. [You can read more about this function here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift).

history.unshift({

arrived: oldRecord.arrived,

left:newDate(Date.now())

});

  The only attribute for a visitor who is not currently logged on is history. So we set the visitor&#39;s new history by utilizing the setVisitor function.

setVisitor(name,{history: history});

return`OK, ${name} is logged out now`;

};

  The log in function has a similar concept except that here it creates a new record with the existing history and an arrived attribute with the current time.

varlogIn=(name)=\&gt;{

var oldRecord =getVisitor(name);

var history;

  When you have multiple conditions, and you only want the first one that is true to be processed, you can use this syntax:
if \&lt;condition A\&gt; \&lt;action A\&gt; else if \&lt;condition B\&gt; \&lt;action B\&gt; else if \&lt;condition C\&gt; \&lt;action C\&gt; … else \&lt;default action\&gt;
 Because of the else if statements, once a condition is evaluated as true the action for it happens and the rest of the conditions are skipped.
 Here we need to check if there is an existing entry before we check if it has an arrived attribute because it is an error to check for attributes of an undefined value.

// First time we see this person

if(oldRecord ===undefined)

history =[];// No history

// Already logged in

elseif(oldRecord.arrived !==undefined)

return`Error, ${name} is already logged in`;

// Not logged in, already exists

else history = oldRecord.history;

setVisitor(name,{

arrived:newDate(Date.now()),

history: history

});

return`OK, ${name} s logged in now`;

};

1.

### Testing

The code above looks like it should work, but it is best to test it before proceeding. For testing purposes, various paths under /test return the results of the above functions. Doing this relies on testFunctions, which is a JSON that has paths and their associated functions. The functions in this object do not receive any parameters, and return the information that is sent to the user. To enable the testing of functions that do require parameters, such as logIn(), they are wrapped in the table within a definition that does provide the necessary parameters. That way, the code that uses the table does not need to specify any parameter values.

var testFunctions =[

The first few lines are simply function names for functions that do not accept parameters. There is no need to wrap them.

{path:&quot;visitorNames&quot;, func: visitorNames},

{path:&quot;currentVisitorNames&quot;, func: currentVisitorNames},

{path:&quot;nonCurrentVisitorNames&quot;, func: nonCurrentVisitorNames},

{path:&quot;currentVisitorList&quot;, func: currentVisitorList},

{path:&quot;currentVisitors&quot;, func: currentVisitors},

The /test/visitors path that we tried earlier does not actually show the output of a function, but a variable. However, the code that uses the table expects a function – so we wrap it in a function.

{path:&quot;visitors&quot;,func:()=\&gt; visitors},

The logIn and logOut functions do get a parameter, a user name. To run the simple tests we need here, we use a fixed username - **Avimelech ben-Gideon**.

{path:&quot;logIn&quot;,func:()=\&gt;logIn(&quot;Avimelech ben-Gideon&quot;)},

{path:&quot;logOut&quot;,func:()=\&gt;logOut(&quot;Avimelech ben-Gideon&quot;)}

];

This is the code that registers the handlers. It prepends /test/ to the path and creates a function that calls the function from the table and then sends the response to the browser.

testFunctions.map((item)=\&gt;

app.get(

`/test/${item.path}`,

/\* @callback \*/function(req, res){

res.send(item.func());

}

)

);

To actually test the application, first go to /test/logOut to log out the non-existent Avimelech ben-Gideon account and see the error code.

![](RackMultipart20210911-4-8gav30_html_fb04d65251dea7ba.png) Figure 11. Test case: logging out without logging in

Then go to /test/logIn twice. The first attempt should succeed and the second one fails.

![](RackMultipart20210911-4-8gav30_html_2ec442dd43ab3823.png) Figure 12. Test case: logging in ![](RackMultipart20210911-4-8gav30_html_4aab4161132fd394.png) Figure 13. Test case: logging in after logging in

Then go to /test/logOut twice to see the first attempt succeeds and the second one fails

![](RackMultipart20210911-4-8gav30_html_c3c31352eb7f2f5f.png) Figure 14. Test case: logging out ![](RackMultipart20210911-4-8gav30_html_dbaa51dbde6429ef.png) Figure 15. Test case: logging out after logging out

After you do these steps, and maybe log in and log out a few more times, go to /test/visitors to see the JSON data for the visitor log and copy paste this into the JSON formatter, you will see something like this:

![](RackMultipart20210911-4-8gav30_html_48ec90cef38a9c63.png)
 Figure 16. Test case: getting visitors&#39; JSON

Finally, you can also look at the other function URLs, such as /test/currentVisitorNames, to see that it shows the correct information. Just Log In/Out and see if the currentVisitorNames variable is updated properly. Note that if you look at those paths on the sample application (link shared above) there might be excess information from other users who might be going through this course and testing it out.

The main data structure of the application is a visitor log. Let&#39;s try it out and see how it looks.

1. You can see the source code with the code that declares and manipulates the visitor log [here](https://github.com/qbzzt/bluemix/blob/master/security/201803/Visitor_Log/02-app.js). Copy this code and replace it with the code in your current **app.js** and then click the **play** button to restart the application.

1. You can see the current visitor log by adding the text: **test/visitors** at the end of your application URL. It will look like this:

 ![](RackMultipart20210911-4-8gav30_html_3e20bbdda59b787a.png)

Figure 22. Browser JSON viewer

The text you see on the page is called **JavaScript Object Notation** ( **JSON** ). Some browsers format it as shown above however sometimes the output might look like this raw data:


 ![](RackMultipart20210911-4-8gav30_html_ef7a7145e00cf653.png)

Figure 23. Unformatted JSON opened in a browser

Then it might be clearer if you useYou can it more readable by using [a JSON formatter such as this one](https://jsonformatter.curiousconcept.com/). Just copy and paste the raw data that you will get (like the one in the figure above) into this link and it will be formatted to something you can understand. It will look like this:

 ![](RackMultipart20210911-4-8gav30_html_80e40128f6c9e448.png)

Figure 24. Expanded JSON

[To see the visitor log for our sample application instance, click here](https://visitor-log-qbzzt.mybluemix.net/test/visitors?cm_mc_uid=62379037222015373600237&amp;cm_mc_sid_50200000=26941741538569905159&amp;cm_mc_sid_52640000=72791401538569905167)To see the visitor log for our sample application instance, [click here](https://visitor-log-qbzzt.mybluemix.net/test/visitors?cm_mc_uid=62379037222015373600237&amp;cm_mc_sid_50200000=26941741538569905159&amp;cm_mc_sid_52640000=72791401538569905167).

1. Let&#39;s try to understand what this log tells us. This visitor log is an **associative array** (also called a **hash table** , or an **object** ). Associative arrays have **key-value** pairs. Instead of storing data in a linear way like with the normal arrays (array [[0] = &quot;Bill Hamm&quot;), here you store the data as a **collection** and assign it one unique value. You can later call these values from anywhere using a particular syntax. The associative array here has **keys** which are visitor names (for example: &quot;Bill Hamm&quot;). The **value** for each of these keys (visitor names) is itself another associative array, which can have two **attributes** ( **keys** ):

Arrivedarrived – The last time the visitor arrived at the office. This attribute does not exist if the visitor is not currently in the office.

Historyhistory – The visitor&#39;s history, an array of associate arrays with the start and end times of previous visits. This attribute does not exist during the first visit to the office.

1. As you can see in the previous figures that we already have some sample data for testing purposes. This data was defined in the code that we used earlier, here is the code snippet:

// Visitors data structure

var visitors = {

&quot;Bill Hamm&quot;: {

arrived: new Date(Date.now() - 1000\*3600\*2)

},

&quot;Deborah Lapidot&quot;: {

arrived: new Date(Date.now() - 1000\*3600),

history: [

{

arrived: new Date(Date.now() - 26\*1000\*3600),

left: new Date(Date.now() - 24\*1000\*3600)

}

]

},

&quot;Ehud ben-Gera&quot;: {

history: [

{

arrived: new Date(Date.now() - (3\*24+3)\*1000\*3600),

left: new Date(Date.now() - (3\*24-1)\*1000\*3600)

},

{

arrived: new Date(Date.now() - (2\*24+2)\*1000\*3600),

left: new Date(Date.now() - (2\*24-5)\*1000\*3600)

}

]

}

};

 Most of it is a standard JavaScript object definition, but the dates, instead of being fixedconstants, are now assigned to a short amount of a fixed time before the application&#39;s starttime before the application was started. Date.now() is the number of milliseconds between now and a fixed point in time (midnight January 1st 1970 GMT). So Bill Hamm&#39;s arrival time is two hours before this code is executed when the application starts. [You can read more about the Date object here](https://www.w3schools.com/jsref/jsref_obj_date.asp).

&quot;Bill Hamm&quot;: {

arrived: new Date(Date.now() - 1000\*3600\*2)

},

###
 Reading the visitor log

When displaying the visitor log, we might want to display all of it, or we might want to display just the current visitors, those that are currently in the office. Also, it can be useful to get the names of all the visitors, all the visitors currently in the office, or all those who currently aren&#39;t, without their full information. These are the functions that implement these requirements:

1. To get the list of visitor names, all we need is to get the **keys** of the visitors object. The function to do this is [Object.keys](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys/). Note that the function syntax here is the new one:

var Function\_Name =,(parameterParameter\_1, Parameter\_2, …, Parameter\_Ns) =\&gt;

{

\&lt;\&lt;Function code goes here\&gt;\&gt; expressions;

}

. This is called an arrow function, it&#39;s the same as the anonymous functions we described earlier except that the syntax contains an arrow here and it&#39;s simpler and more concise. In this particular case, there are no parameters:.

var visitorNames = () =\&gt; {

return Object.keys(visitors);

};

1. To get a subset (either those who are in the office or those who aren&#39;t), use the filter() function. It Filter functions returns an array of elements that pass a particular test. It gets one parameter, a function. This function gets an item from the list as a parameter and returns whether or not that item should be a member of the filtered list. In our case we are trying to filter out all the visitor names that have the arrived in the office (in coding: those whose arrived values are not equal to undefined). This function is an array method (so you can call it on any list, such as the one returned by visitorNames).

The function definition is simplified. When a function literal is a single expression, there is no need to enclose it in curly brackets ({}) and have a return statement. You can just enter the expression.

var currentVisitorNames = () =\&gt; {

    return visitorNames().filter((name) =\&gt; visitors[name].arrived !== undefined);

};

By using the filter() function we just got the list of names who have arrived in the office but not their details that were there in the default visitor log. It is a bit more complicated to get the list of current visitors with their information, with the names as keys.

1. The first step is inThen next step is to create list with of currently present visitors called currentVisitorList. This function uses the map() function to retrieve the information for each user in the list of current visitors. This function receives a function as a parameter, similar to filter() function. However, instead of deciding whether a value will be in the output or not, the function in map is used to transform the values:

- . It creates a new array
- usingThis array is populated with the mapping function results
- from the function that is mapping whateverEvery time the mapping function is executed, it receives the data of the currently present visitor and puts it an object names are there in the current visitor list to the one in the original visitors list to get their information.
- Afterwards, Tthese transformed valuesobjects are turned intoput in a list in the same order as the original values.

[You read about this function hereYou can learn more about this function here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map).

 In this case, for each name we get a structure with the user information. For example, if you add /test/currentVisitorList at the end of your application URL, you will get the list of current visitors with their information that we got using the mapping function.

var currentVisitorList = () =\&gt; {

return currentVisitorNames().map((name) =\&gt; {

var retVal = {};

retVal[name] = visitors[name];

return retVal;

});

};

 ![](RackMultipart20210911-4-8gav30_html_20cb492f2f2ab155.png)

Figure 25. currentVisitorList

This list has the information we need,. but However each user is in a separate object in a list. It makes a lot more sense to use the same format we use in the visitors variable, one object with each user being a separate attribute

1. . To do thatThe final step is to turn the list of current visitors in a single object., To achieve that, we use the reduce() function to turn the list into a single object. If the list it receives has one item, it returns that item. If it has two items, it runs the parameter function on them and returns the result. If there are more, it runs the parameter function on two of them, then on that result and another one, until there is only a single value left. [You can read more about the function here](https://www.w3schools.com/jsref/jsref_reduce.asp).

var currentVisitors = () =\&gt; {

return currentVisitorList().reduce((a, b) =\&gt; {

var bKey = Object.keys(b)[0];

a[bKey] = b[bKey];

return a;

});

};

 To create the combined object, we first need the key of the new object, the one from the list which only has a single attribute for a single user (var bKey = Object.keys(b)[0];).

 We add this value to the original object, the one in which we accumulate all the users (a[bKey] = b[bKey];). Then we finally return it.

### Updating the visitor log

There are two way to make modifications to the visitor log. A user may be logged in when the enter the office or logged out when they leave..

For these functions we have a **get** function and a **set** function to interact with the visitors variable. The get function gets the details of a visitor when it is given a name and the set function sets a new visitor or updates existing details of a visitor when given a name and its value./ The purpose of these functions is to make it easy to modify the application to use a different data storage, for example a database, in the future.

var getVisitor = (name) =\&gt; visitors[name];

var setVisitor = (name, values) =\&gt; visitors[name] = values;

Let us look at the logOutlogout() function now by breaking it down line by line:

1.
2. The log out function is relatively simple. FirstFirst, we store the details of that particular visitor in a new variable oldRecord.

var logOut = (name) =\&gt; {
3.

var oldRecord = getVisitor(name);

1.

 Then we check if the visitor even exists, if the name is not found, then we return text saying that there is an error.

if (oldRecord === undefined)

return `Error, ${name} is unknown`;
if (oldRecord === undefined)

return `Error, ${name} is unknown`;

1.
 Next, we check whether the user has an arrived attribute. If the user doesn&#39;t have it, this user is not currently in the office and cannot be logged out. Report an error.

if (oldRecord.arrived === undefined)

return `Error, ${name} is not logged in`;

1.
 If the is no error till now it means the visitor is in the system and is logged in. Then the only attribute in the old record that is still relevant is history. We need to keep it and add a new value to it. However, if this is the first visit there might be no history yet. In such a case, the history is empty..

2.

var history = oldRecord.history;

// If this is the first visit

if (history === undefined)

history = [];

1. The unshift function adds a new value at the beginning of an array. This is the behavior we want here, because the latest visits are more likely to be relevant, so it is best if the array is sorted in reverse chronological order. [You can read more about this function here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift)..

history.unshift({

    arrived: oldRecord.arrived,

    left: new Date(Date.now())

});

1. The only attribute for a visitor who is not currently logged on is history. So we set the visitor&#39;s new history by utilizing the setVisitor function..

setVisitor(name, {history: history});

    return `OK, ${name} is logged out now`;

};

1. The log in function has a similar concept except that here it creates a new record with the existing history and an arrived attribute with the current time..

var logIn = (name) =\&gt; {

    var oldRecord = getVisitor(name);

    var history;

1. When you have multiple conditions, and you only want the first one that is true to be processed, you can use this syntax:

if \&lt;condition A\&gt; \&lt;action A\&gt; else if \&lt;condition B\&gt; \&lt;action B\&gt; else if \&lt;condition C\&gt; \&lt;action C\&gt; … else \&lt;default action\&gt;

Because of the else if statements, once a condition is evaluated as true the action for it happens and the rest of the conditions are skipped.

Here we need to check if there is an existing entry before we check if it has an arrived attribute because it is an error to check for attributes of an undefined value.

    // First time we see this person

    if (oldRecord === undefined)

        history = [];   // No history

    // Already logged in

    else if (oldRecord.arrived !== undefined)

        return `Error, ${name} is already logged in`;



    // Not logged in, already exists

    else history = oldRecord.history;

    setVisitor(name, {

        arrived: new Date(Date.now()),

        history: history

    });

    return `OK, ${name} is logged in now`;

};

### Testing

The code above looks like it should work, but it is best to test it before proceeding. For testing purposes, various paths under /test return the results of the above functions. Doing this relies on testFunctions, which is a table JSON that has paths and their associated functions. The functions in this table object do not receive any parameters, and return the information to that is send sent to the user. To enable the testing of functions that do require parameters, such as logIn(), they are wrapped in the table within a definition that does provide the necessary parameters. That way, the code that uses the table does not need to specify any parameter values.

var testFunctions = [

The first few lines are simply function names for functions that do not accept parameters. There is no need to wrap them.

{path: &quot;visitorNames&quot;, func: visitorNames},

{path: &quot;currentVisitorNames&quot;, func: currentVisitorNames},

{path: &quot;nonCurrentVisitorNames&quot;, func: nonCurrentVisitorNames},

{path: &quot;currentVisitorList&quot;, func: currentVisitorList},

{path: &quot;currentVisitors&quot;, func: currentVisitors},

The /test/visitors path that we tried earlier does not actually show the output of a function, but a variable. However, the code that uses the table expects a function – so we wrap it in a function.

{path: &quot;visitors&quot;, func: () =\&gt; visitors},

The logIn and logOut functions do get a parameter, a user name. To run the simple tests we need here, we use a fixed user name - **Avimelech ben-Gideon**.

 {path: &quot;logIn&quot;, func: () =\&gt; logIn(&quot;Avimelech ben-Gideon&quot;)},

    {path: &quot;logOut&quot;, func: () =\&gt; logOut(&quot;Avimelech ben-Gideon&quot;)}

];

This is the code that registers the handlers. It prepends /test/ to the path and creates a function that calls the function from the table and then sends the response to the browser.

testFunctions.map((item) =\&gt;

    app.get(

        `/test/${item.path}`,

        /\* @callback \*/ function(req, res) {

            res.send(item.func());

        }

    )

);

To actually test the application, first go to [/test/logOut](https://visitor-log-qbzzt.mybluemix.net/test/logOut)/test/logOut to log out the non-existent Avimelech ben-Gideon account and see the error code.

![](RackMultipart20210911-4-8gav30_html_82d07043bc4e7f8b.png)

Figure 26. Test case: logging out without logging in

Then go to [/test/logIn](https://visitor-log-qbzzt.mybluemix.net/test/logIn)/test/logIn twice. The first attempt should succeed and the second one fails.

![](RackMultipart20210911-4-8gav30_html_e94dc36cab53385c.png)

Figure 27. Test case: logging in

![](RackMultipart20210911-4-8gav30_html_2d4e8bced42de18e.png)

Figure 28. Test case: logging in after logging in

Then go to [/test/logOut](https://visitor-log-qbzzt.mybluemix.net/test/logOut)/test/logOut/test/logOut twice to see the first attempt succeeds and the second one fails

![](RackMultipart20210911-4-8gav30_html_c03c17a9634ab80d.png)

Figure 29. Test case: logging out

![](RackMultipart20210911-4-8gav30_html_55e30c3779c5c80c.png)

Figure 30. Test case: logging out after logging out

After you do these steps, and maybe [log in](https://visitor-log-qbzzt.mybluemix.net/test/logIn)log in and log [ouloig t](https://visitor-log-qbzzt.mybluemix.net/test/logOut)out a few more times, go to [/test/visitors](https://visitor-log-qbzzt.mybluemix.net/test/visitors)/test/visitors to see the JSON data for the visitor log and copy paste this into the JSON formatter you will see something like this:

 ![](RackMultipart20210911-4-8gav30_html_2fddef0bceba1da8.png)

Figure 31. Test case: _getting visi_tors&#39; JSON

Finally, you can also look at the other function URLs, such as [/test/currentVisitorNames](https://visitor-log-qbzzt.mybluemix.net/test/currentVisitorNames)/test/currentVisitorNames, to see that it shows the correct information. Just Log In/LogOut and see if the currentVisitorNames variable is updated properly.

Note that if you look at those paths on the sample application there might be excess information from other readers of this article.

## User interfaceInterface

Now since we have tested our application and the basic functionality is working, lets add some basic UI elements to make it a proper web application with a User Interface.

1. Replace the code in your **app.js** again [with the file found in this github link](https://github.com/qbzzt/bluemix/blob/master/security/201803/Visitor_Log/03-app.js). It mostly has the same code as the previous file that we just went through, except that now we are adding some lines of code for the User Interface.
2. Once again click on the raw button, copy the entire code here, remove all the code in your app.js file and paste this new code there. Once done go ahead and press the play button to redeploy the app. ![](RackMultipart20210911-4-8gav30_html_34e98e0c6f1779a0.png) Figure 1. Raw button

 ![](RackMultipart20210911-4-8gav30_html_98c3d04746ccd60f.png)
 Figure 2. Copy code ![](RackMultipart20210911-4-8gav30_html_b13f73f11df606cf.png) Figure 3. Replace current code and redeploy

3. If it asks for a confirmation again, proceed with it. ![](RackMultipart20210911-4-8gav30_html_32e59947e716e3b5.png) Figure 4. Confirmation box
4. After you have replaced the code, add /visitors at the end of your application URL to see the full visitor list. ![](RackMultipart20210911-4-8gav30_html_7512d14dce583a85.png) Figure 5. List of all visitors in a table format
5. You can click on the details button as shown above to see the **arrived** and **left** times for every visitor. ![](RackMultipart20210911-4-8gav30_html_a04f9a850c688c66.png) Figure 6. Details of a visitor
6. Go to /currentVisitors to see the current visitor list who haven&#39;t logged out. ![](RackMultipart20210911-4-8gav30_html_20ca7b555843c75a.png) Figure 7. List of current visitors in a table format
7. Add users by logging them in with /login. Add any name of the user of your choosing and press enter. ![](RackMultipart20210911-4-8gav30_html_904bd6d2dd9aa6ae.png) Figure 8. Logging in users ![](RackMultipart20210911-4-8gav30_html_f0c8a9e377bd46f6.png) Figure 9. Successfully logged in

8. Remove users by logging them out by adding /logout at the end of your main app URL. Just click on any user you would like to logout. ![](RackMultipart20210911-4-8gav30_html_837d2922d5081608.png)
 Figure 10. Logging out users ![](RackMultipart20210911-4-8gav30_html_ba210a97175fa089.png) Figure 11. Successfully logged out
9. To see the entire user interface, go to /index.html of your application. ![](RackMultipart20210911-4-8gav30_html_b39903a2862ae371.png)
 Figure 12. Main page

Great! We have our basic UI application running. Let&#39;s try to understand the code now.

The first difference is this instruction to the Eslint to ignore unused parameters. This is because the /\* callback \*/ directive (ignore unused parameters only for this function call).

/\* eslint-disable no-unused-params \*/

It is useful to know how long a visitor has been in the office, but a big number such as 5000 seconds is hard to interpret. This function below (tdiffToString) turns a time difference in milliseconds to a readable string. The input is milliseconds (msec) because that&#39;s the standard in most JavaScript functions that relate to time. In the first line of the function we turn the milliseconds to seconds.

// Given a time difference in milliseconds, return a string

// with the approximate value

vartdiffToString=(msec)=\&gt;{

var sec = msec/1000;

Then we use an if statement to determine if the number of seconds is less than 60. If it is, the application returns a properly labeled number of seconds. So for example, if the user was in for 20 seconds the if statement will return &quot;60 seconds&quot;. But what if the user was in for just one second? How do we switch the word &quot;seconds&quot; to &quot;second&quot; without an &quot;s&quot;? For this we use the [ternary operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator) to either add an &quot;s&quot; for plural or not. This operator is basically a shortcut for an if statement which takes three parameters. If the first parameter (less than 2 seconds (sec \&lt; 2)) is true, it returns the second parameter (an empty string &quot;&quot;). If the first parameter is false, which means that seconds is greater than 2, we need to use the plural, the operator returns the third parameter, the plural &quot;s.&quot; which is added to the word &quot;second&quot;.

if(sec \&lt;60)

return sec +&quot; second&quot;+(sec \&lt;2?&quot;&quot;:&quot;s&quot;);

If the number of seconds is less than 60, the function has already returned as shown above. If the number of seconds is between 60 and 3600 (an hour), we need to return the number of minutes in the time interval. Note the use of [Math.floor()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/floor), it takes any number (5.65 for example) and returns the largest whole number before it (5). It is necessary because we want to avoid reporting values like 5.23544 minutes which in our case will be &quot;5 minutes&quot;. Then the last part (sec \&lt; 60\*2 ? &quot;&quot; : &quot;s&quot;); basically works the same way as before except that here it checks if seconds are less than 120 in which case it will only be &quot;1 minute&quot; without an &quot;s&quot;.

if(sec \&lt;3600)

return Math.floor(sec/60)+&quot; minute&quot;+(sec \&lt;60\*2?&quot;&quot;:&quot;s&quot;);

The rest of the function, for hours and days, operates the same way.

…

};

This is the first function that produces HTML. The user interface displays the history (arrivals, departures, and the intervening time when we click on the details tab) in an [HTML table](https://www.w3schools.com/html/html_tables.asp) (we saw this table in the previous course)– and this function produces the rows in that table.

// Given a history entry (arrived and left times), create a table row with

// that information

varhistEntryToRow=(entry)=\&gt;{

return`\&lt;tr\&gt;

\&lt;td\&gt;${entry.arrived}\&lt;/td\&gt;

\&lt;td\&gt;${entry.left}\&lt;/td\&gt;

\&lt;td\&gt;${tdiffToString(entry.left-entry.arrived)}\&lt;/td\&gt;

\&lt;/tr\&gt;`;

};

The next function produces an entire table (if there is anything to produce, otherwise it just returns an empty string).

// Given a history, create a table with it

varhistToTable=(history)=\&gt;{

if(history ===undefined)

return&quot;&quot;;

if(history.length ===0)

return&quot;&quot;;

People don&#39;t always want to see the history. By enclosing it in [a details tag](https://www.w3schools.com/tags/tag_details.asp) we hide the history until a user decides to open it. [The style attribute](https://www.w3schools.com/html/html_styles.asp) allows us to specify the background color to make the history tables distinct from the rest of the visitor information (which is also displayed in table form).

return`\&lt;details\&gt;

\&lt;table border style=&quot;background-color: yellow&quot;\&gt;

\&lt;tr\&gt;

\&lt;th\&gt;

Arrived

\&lt;/th\&gt;

\&lt;th\&gt;

Left

\&lt;/th\&gt;

\&lt;th\&gt;

Time here

\&lt;/th\&gt;

\&lt;/tr\&gt;

${history.map(histEntryToRow).reduce((a, b) =\&gt; a+b)}

\&lt;/table\&gt;

\&lt;/details\&gt;`;

};

The next two functions, userToRow and usersToTable, are very similar to the way we create the history table, so we can skip going over them.

Next, visitorsHTML and currentVisitorsHTML add a heading and create the table with the appropriate user names list. Again, those functions are so similar that it is enough to see one of them.

varvisitorsHTML=()=\&gt;{

return`

\&lt;h2\&gt;Current Visitor List\&lt;/h2\&gt;

${usersToTable(visitorNames())}

`;

};

This function creates a login form. It uses an [HTML form](https://www.w3schools.com/html/html_forms.asp) with the **GET** method. This means the parameters (in this case there is only one, user) are going to be encoded in the URL. The login attribute gives the path for the handler, which you will see later in the article.

varloginForm=()=\&gt;{

return`\&lt;h2\&gt;Log in a visitor\&lt;/h2\&gt;

\&lt;form method=&quot;get&quot; action=&quot;login&quot;\&gt;

Visitor to log in: \&lt;input type=&quot;text&quot; name=&quot;user&quot;\&gt;

\&lt;/form\&gt;`;

};

There is one substantial difference between the login form and the logout form. There is no way to know in advance which visitor is going to be logged in. It may even be somebody completely new. However, the only visitors that can be logged out are those who are currently logged in. This lets us show a list and have the user choose from it.

varlogoutForm=()=\&gt;{

if(currentVisitorNames().length ===0)

return&quot;No users to log out&quot;;

return `

\&lt;h2\&gt;Log out a visitor\&lt;/h2\&gt;

\&lt;ul\&gt;

${currentVisitorNames()

Instead of creating a form with an input field, I decided to use links. We can do that, and simulate a GET form, because of the way a GET form returns its parameters. You have the usual URL (http://\&lt;hostname\&gt;/\&lt;\&lt;path\&gt;) followed by a question mark, then \&lt;parameter\&gt;=\&lt;value\&gt; pairs, separated by ampersands (&amp;). The value might include characters that have a special meaning in URLs (such the ampersand), so they are escaped. This is the role of [the encodeURI function](https://www.w3schools.com/jsref/jsref_encodeURI.asp).

.map(name=\&gt;`\&lt;li\&gt;

\&lt;a href=&quot;logout?user=${encodeURI(name)}&quot;\&gt;${name}\&lt;/a\&gt;

\&lt;/li\&gt;`)

.reduce((a,b)=\&gt; a + b)}

\&lt;/ul\&gt;`;

};

This function takes text, such as the HTML produced by the above functions, and turns it to a complete web page.

varembedInHTML=(str)=\&gt;{

return`\&lt;html\&gt;\&lt;body\&gt;${str}\&lt;/body\&gt;\&lt;/html\&gt;`;

};

These two calls call the proper function to create the heading and table, embed it within a page, and respond.

app.get(&quot;/visitors&quot;,(req, res)=\&gt;{

res.send(embedInHTML(visitorsHTML()));

});

app.get(&quot;/currentVisitors&quot;,(req, res)=\&gt;{

res.send(embedInHTML(currentVisitorsHTML()));

});

These two calls are the form handlers. The parameters submitted to the form using the GET method are available in req.query. If there is no user, send the form. If there is a user, process the command for that user.

app.get(&quot;/login&quot;,(req, res)=\&gt;{

if(req.query.user ===undefined)

res.send(embedInHTML(loginForm()));

else

res.send(logIn(req.query.user));

});

app.get(&quot;/logout&quot;,(req, res)=\&gt;{

if(req.query.user ===undefined)

res.send(embedInHTML(logoutForm()));

else

res.send(logOut(req.query.user));

});

This app.get call shows everything in the application. Instead of a path there is a list of paths, which Express interprets as &quot;this handler applies to everything in this list.&quot;

app.get([&quot;/index.html&quot;,&quot;/&quot;],(req, res)=\&gt;{

res.send(embedInHTML(`

${loginForm()}

\&lt;hr /\&gt;

${logoutForm()}

\&lt;hr /\&gt;

${currentVisitorsHTML()}

\&lt;hr /\&gt;

${visitorsHTML()}

`));

});

If we keep this call it overrides the handler we registered – so I commented it out.

/\*

// serve the files out of ./public as our main files

app.use(express.static(\_\_dirname + &#39;/public&#39;));

\*/

Now since we have tested our application and the basic functionality is working, lets add some basic UI elements to make it a proper application.

1. Replace the code in your **app.js** again with the file found [the file found herehere](https://github.com/qbzzt/bluemix/blob/master/security/201803/Visitor_Log/03-app.js). It has the same code as the previous file that we just went through except that now we are adding some lines of code for the UI.

2. After you have replaced the code, go to /visitors on your application ([or the sample application](https://visitor-log-qbzzt.mybluemix.net/visitors)) to see the full visitor list.

 ![](RackMultipart20210911-4-8gav30_html_1bd36527b015f6fa.png)

Figure 32. List of all visitors in a table format

1.

 You can click on the details button as shown above to see the **arrived** and **left** times for every visitor.

2. Go to [/currentVisitors](https://visitor-log-qbzzt.mybluemix.net/currentVisitors)/currentVisitors to see the current list.

 ![](RackMultipart20210911-4-8gav30_html_74df8b22d2aaee54.png)

Figure 33. List of current visitors in a table format

1. Add users by logging users in with [/login](https://visitor-log-qbzzt.mybluemix.net/login)/login and logging out with [/logout](https://visitor-log-qbzzt.mybluemix.net/logout)/logout.

2. To see the entire user interface, go to [/index.html](https://visitor-log-qbzzt.mybluemix.net/)/index.html.

 ![](RackMultipart20210911-4-8gav30_html_979bbbcf8c853fad.png)

Figure 34. Main page

Great! We have our basic UI application running. Let&#39;s try to understand the code now.

 The first difference is this instruction to the Eslint to ignore unused parameters. This is because the /\* callback \*/ directive (ignore unused parameters only for this function call).

/\* eslint-disable no-unused-params \*/

It is useful to know how long a visitor has been in the office, but a big number such as 5000 seconds is hard to interpret. This function below (tdiffToString) turns a time difference in milliseconds to a readable string. The input is milliseconds (msec) because that&#39;s the standard in most JavaScript functions that relate to time. In the first line of the function we turn the milliseconds msec to seconds.

// Given a time difference in milliseconds, return a string

// with the approximate value

var tdiffToString = (msec) =\&gt; {

    var sec = msec/1000;

Then we use an IFif statement to determine determine if If the number of seconds is less than 60. If it is, the application returns a properly labeled number of seconds. So for example, if the user was in for 20 seconds the if statement will return &quot;60 seconds&quot;. But what if the user was in for just one second? How do we switch the word &quot;seconds&quot; to &quot;second&quot; without an &quot;s&quot;? For this we use the [trinary operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator) to either add an &quot;s&quot; for plural or not. This operator is basically a shortcut for an if statement which takes three parameters. If the first parameter (less than 2 seconds sec \&lt; 2) is true, it returns the second parameter (an empty string &quot;&quot;). If the first parameter is false, which means that seconds is greater than 2, we need to use the plural, the operator returns the third parameter, the plural &quot;s.&quot; which is added to the word &quot;second&quot;.

if (sec \&lt; 60)

    return sec + &quot; second&quot; + (sec \&lt; 2 ? &quot;&quot; : &quot;s&quot;);

If the number of seconds is less than 60, the function has already returned as shown above. If the number of seconds is the between 60 and 3600 (an hour), we need to return the number of minutes in the time interval. Note the use of [Math.floorMath.floor()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/floor), it takes any number (5.65 for example) and returns the largest whole number before it (5). It is necessary because we want to avoid reporting values like 5.23544 minutes which in our case will be &quot;5 minutes&quot;. Then the last part (sec \&lt; 60\*2 ? &quot;&quot; : &quot;s&quot;); basically works the same way as before except that here it checks it seconds are less than 120 in which case it will onle only be &quot;one 1 minute&quot; without an &quot;s&quot;.

if (sec \&lt; 3600)

    return Math.floor(sec/60) + &quot; minute&quot; + (sec \&lt; 60\*2 ? &quot;&quot; : &quot;s&quot;);

The rest of the function, for hours and days, operates the same way.

…

};

This is the first function that produces HTML. The user interface displays the history (arrivals, departures, and the intervening time when we click on the details tab) in an [HTML table](https://www.w3schools.com/html/html_tables.asp) (we saw this table in the previous course)– and this function produces the rows in that table.

// Given a history entry (arrived and left times), create a table row with

// that information

var histEntryToRow = (entry) =\&gt; {

    return `\&lt;tr\&gt;

        \&lt;td\&gt;${entry.arrived}\&lt;/td\&gt;

        \&lt;td\&gt;${entry.left}\&lt;/td\&gt;

        \&lt;td\&gt;${tdiffToString(entry.left-entry.arrived)}\&lt;/td\&gt;

        \&lt;/tr\&gt;`;

};

The next function produces an entire table (if there is anything to produce, otherwise it just returns an empty string).

// Given a history, create a table with it

var histToTable = (history) =\&gt; {

    if (history === undefined)

        return &quot;&quot;;

    if (history.length === 0)

        return &quot;&quot;;

People don&#39;t always want to see the history. By enclosing it in [a details tag](https://www.w3schools.com/tags/tag_details.asp) we hide the history until a user decides to open it. [The style attribute](https://www.w3schools.com/html/html_styles.asp) allows us to specify the background color to make the history tables distinct from the rest of the visitor information (which is also displayed in table form).

    return `\&lt;details\&gt;

        \&lt;tableborder style=&quot;background-color: yellow&quot;\&gt;

            \&lt;tr\&gt;

                \&lt;th\&gt;

                    Arrived

                \&lt;/th\&gt;

                \&lt;th\&gt;

                    Left

                \&lt;/th\&gt;

                \&lt;th\&gt;

                    Time here

                \&lt;/th\&gt;

            \&lt;/tr\&gt;

            ${history.map(histEntryToRow).reduce((a, b) =\&gt; a+b)}

        \&lt;/table\&gt;

    \&lt;/details\&gt;`;

};

The next two functions, userToRow and usersToTable, are very similar to the way we create the history table, so we can skip going over them.

 Next, visitorsHTML and currentVisitorsHTML add a heading and create the table with the appropriate user names list. Again, those functions are so similar that it is enough to see one of them.

var visitorsHTML = () =\&gt; {

    return `

                \&lt;h2\&gt;Current Visitor List\&lt;/h2\&gt;

                    ${usersToTable(visitorNames())}

        `;

};

This function creates a login form. It uses an [HTML form](https://www.w3schools.com/html/html_forms.asp) with the **GET** method. This means the parameters (in this case there is only one, user) are going to be encoded in the URL. The login attribute gives the path for the handler, which you will see later in the article.

var loginForm = () =\&gt; {

    return `\&lt;h2\&gt;Log in a visitor\&lt;/h2\&gt;

            \&lt;formmethod=&quot;get&quot;action=&quot;login&quot;\&gt;

                Visitor to log in: \&lt;inputtype=&quot;text&quot;name=&quot;user&quot;\&gt;

            \&lt;/form\&gt;`;

};

There is one substantial difference between the login form and the logout f&quot;form. &quot; There is no way to know in advance which visitor is going to be logged in. It may even be somebody completely new. However, the only visitors that can be logged out are those who are currently logged in. This lets us show a list and have the user choose from it.

var logoutForm = () =\&gt; {

    if (currentVisitorNames().length === 0)

        return &quot;No users to log out&quot;;

    return `

        \&lt;h2\&gt;Log out a visitor\&lt;/h2\&gt;

        \&lt;ul\&gt;

            ${currentVisitorNames()

Instead of creating a form with an input field, I decided to use links. We can do that, and simulate a GET form, because of the the way a GET form returns its parameters. You have the usual URL (http://\&lt;hostname\&gt;/\&lt;path\&gt;) followed by a question mark, then \&lt;parameter\&gt;=\&lt;value\&gt; pairs, separated by ampersands (&amp;). The value might include characters that have a special meaning in URLs (such the ampersand), so they are escaped. This is the role of [the encodeURI function](https://www.w3schools.com/jsref/jsref_encodeURI.asp).

                .map(name =\&gt; `\&lt;li\&gt;

                    \&lt;ahref=&quot;logout?user=${encodeURI(name)}&quot;\&gt;${name}\&lt;/a\&gt;

                    \&lt;/li\&gt;`)

                .reduce((a,b) =\&gt; a + b)}

        \&lt;/ul\&gt;`;

};

This function takes text, such as the HTML produced by the above functions, and turns it to a complete web page.

var embedInHTML = (str) =\&gt; {

    return `\&lt;html\&gt;\&lt;body\&gt;${str}\&lt;/body\&gt;\&lt;/html\&gt;`;

};

These two calls call the proper function to create the heading and table, embed it within a page, and respond.

app.get(&quot;/visitors&quot;, (req, res) =\&gt; {

    res.send(embedInHTML(visitorsHTML()));

});

app.get(&quot;/currentVisitors&quot;, (req, res) =\&gt; {

    res.send(embedInHTML(currentVisitorsHTML()));

});

These two calls are the form handlers. The parameters submitted to the form using the GET method are available in req.query. If there is no user, send the form. If there is a user, process the command for that user.

app.get(&quot;/login&quot;, (req, res) =\&gt; {

    if (req.query.user === undefined)

        res.send(embedInHTML(loginForm()));

    else

        res.send(logIn(req.query.user));

});

app.get(&quot;/logout&quot;, (req, res) =\&gt; {

    if (req.query.user === undefined)

        res.send(embedInHTML(logoutForm()));

    else

        res.send(logOut(req.query.user));

});

This app.get call shows everything in the application. Instead of a path there is a list of paths, which Express interprets as &quot;this handler applies to everything in this list.&quot;

app.get([&quot;/index.html&quot;, &quot;/&quot;], (req, res) =\&gt; {

app.get([&quot;/index.html&quot;, &quot;/&quot;], (req, res) =\&gt; {

    res.send(embedInHTML(`

        ${loginForm()}

        \&lt;hr/\&gt;

        ${logoutForm()}

        \&lt;hr/\&gt;

        ${currentVisitorsHTML()}

        \&lt;hr/\&gt;

        ${visitorsHTML()}

    `));

});

If we keep this call it overrides the handler we registered – so I commented it out.

/\*

// serve the files out of ./public as our main files

app.use(express.static(\_\_dirname + &#39;/public&#39;));

\*/

## Database

There is one problem with the application that we have completed till now. Every time we restarted the app, it loses all the visitor log and starts afresh. To solve this, we need to store the visitor log in a Cloudant database.

In this module we will create a very simple database where the **visitor name** will be the key, and the **data (history and arrival time and date)** is the value.

### Create the database

Follow these steps to create the database:

1. Log in to the [IBM Cloud](https://cloud.ibm.com/), and click **Catalog** on the top. ![](RackMultipart20210911-4-8gav30_html_adade98b822d11a8.png) Figure 1. IBM Cloud catalog
2. Click on **Services** on the left navigation bar, then click on **Databases** and then finally on **Cloudant**. ![](RackMultipart20210911-4-8gav30_html_5d629b9b9f5072e6.png) Figure 2. Services
3. Once again, we choose our region as **London** , but make sure you choose the right region according to what you have chosen in the past for other services. Also, make sure that the free version (Lite) is selected and then go ahead and click on **create**. You can leave all the other fields as default. ![](RackMultipart20210911-4-8gav30_html_8038cd5fc4624d6c.png) Figure 3. Configuring Cloudant DB
4. It might take some time for the cloudant service to be created. As you can see in the image below, it shows provision in process. Wait for sometime for it to complete. If the status doesn&#39;t change in a few minutes you can refresh the current page and check again. ![](RackMultipart20210911-4-8gav30_html_b0dad1a6502c31ea.png) Figure 4. Provisioning Cloudant DB
5. Once its ready you will see the status change to **Active** as shown below. Now you can safely click on your cloudant service to get started. ![](RackMultipart20210911-4-8gav30_html_29d6c2e96450b4fa.png) Figure 5. Cloudant active
6. Click on **Service credentials** in the left navigation bar and then click the **New credential +** button. ![](RackMultipart20210911-4-8gav30_html_c1a3c7e869e259e5.png) Figure 6. Setting up Cloudant DB credentials
7. Name the new credential visitor-log and leave everything else as default. Click **Add**. ![](RackMultipart20210911-4-8gav30_html_7addc7c9781f1268.png) Figure 7. Setting up Cloudant DB credentials
8. In the credential list, click on the down arrow to view the credentials you just created. Click the copy/duplicate icon at the right to copy the credentials and then paste it to a text file (we will be using this later). ![](RackMultipart20210911-4-8gav30_html_35a99537ce5d0e8e.png) Figure 8. Cloudant DB credentials

9. In the left menu bar, click **Manage**. Once the overview page opens, click the **Launch Dashboard** button. ![](RackMultipart20210911-4-8gav30_html_286c554099620075.png) Figure 9. Cloudant dashboard
10. In the left menubar, click the **Databases** icon. ![](RackMultipart20210911-4-8gav30_html_3e87bfeff4e2d5ad.png)
 Figure 10. Cloudant databases&#39; window

11. Then click **Create Database** in the upper right, name your database visitor-log, select the **Non-partitioned** option and click **Create**. ![](RackMultipart20210911-4-8gav30_html_432900a71e8fc2b2.png) Figure 11. Creating a database
12. Keep the Cloudant tab open and in another tab go back to the application development environment and open the file called **package.json**.
13. In the dependencies object, add a comma (,) and then a line for the Cloudant package (&quot;@cloudant/cloudant&quot;: &quot;latest&quot;).

&quot;@cloudant/cloudant&quot;:&quot;latest&quot;

1. After you finish, your file will look like this with the new line added: ![](RackMultipart20210911-4-8gav30_html_6af3fe466fd5820.png) Figure 12. package.json

### Use the database

1. To use the database, replace **app.js** once again with [the code found in this github file](https://github.com/AbdullahTasleem/visitor-logging-course/blob/master/Third%20(db)%20app.js). Again, it uses almost the same data definitions and user interface, so it won&#39;t look different. But there is some additional code for integrating the database so if you now restart the application, the information will not be lost and will be stored in your cloudant database as key value pairs.
 The only thing you need to add before re-deploying the app is to add the Cloudant credentials you copied earlier into this variable:
2. var cloudantCred ={
3. \&lt;\&lt;\&gt;\&gt;

};

 Delete the part with \&lt;\&lt;\&gt;\&gt; and paste your credentials, it should look like this: ![](RackMultipart20210911-4-8gav30_html_4a3c5f5717d133d2.png) Figure 13. Adding Cloudant credentials to the application

 Go ahead and re-deploy the application by clicking on the play button. Wait for the green button to appear, until then it will show a loading sign. ![](RackMultipart20210911-4-8gav30_html_c3138af45fa42fb1.png) Figure 14.Redeploying the app ![](RackMultipart20210911-4-8gav30_html_900c33bd26b1233.png) Figure 15. Deploying

 Let&#39;s try one last time to use our app and see how the data is stored in the database. Once the app is redeployed, open it again, but just your main URL and add log in a new visitor. ![](RackMultipart20210911-4-8gav30_html_84bfb425a7f63bea.png)
 Figure 16. Logging in a new visitor

 Once you press enter you should see the successful login message as shown below. ![](RackMultipart20210911-4-8gav30_html_b623f250ec10db9e.png) Figure 17. New visitor successful login

 Go back to the main application page and see if the new user has been added and also try to log the user out by clicking on the user&#39;s name. ![](RackMultipart20210911-4-8gav30_html_ae3ebd790303e97d.png)
 Figure 18. Logging out the new visitor

 Go back to the tab where you have the cloudant open and refresh the page. You should see one doc added. ![](RackMultipart20210911-4-8gav30_html_1a16999a43a8dc6f.png) Figure 19. New database doc added

 Open the visitor-log database and click on the JSON button, you should be able to see your new user added here. Now even if you restart your application, the new user will always be there. ![](RackMultipart20210911-4-8gav30_html_b3207e2a00d46fe9.png) Figure 20. New entry in the database

 This credential is to connect to the database management system (uses the URL and apikey that you added in the cloudantCred variable), and then specifies which database you are going to use (in our case the visitor-log database):

// Connect to the database

var Cloudant =require(&#39;@cloudant/cloudant&#39;);

var cloudant =newCloudant({ url: cloudantCred.url, plugins:{ iamauth:{ iamApiKey: cloudantCred.apikey }}});

var mydb = cloudant.db.use(&quot;visitor-log&quot;);

  There are two ways we can store the information in the database. One would be to put the entire visitors data structure in a single database entry (called document in Cloudant). The other is to have a separate document for each visitor name. For this introductory course, we will use the first method. It is less efficient, but [it will work for up to 1 MB](https://console.bluemix.net/docs/services/Cloudant/api/document.html#documents). The major advantage of this approach is that we can use the application logic developed previously with almost no change. We can continue to keep the visitors data structure as a variable.

 The same Cloudant database could be used by multiple applications at the same time. To avoid one application&#39;s interference with another, it uses a revision system. Every document has a \_rev value with the current revision. When you update a document, you provide the revision you&#39;re updating. If it changed from the time you read it, the revision is different causing the update to fail—this requires us to have a variable to hold the current revision.

var dbRev =&quot;&quot;;

  This function updates the visitor log on the database.

varupdateVisitors=()=\&gt;{

The data to update always includes \_id, the key, and the actual value. It usually also includes \_rev, the revision. The exception is when creating a new entry.

var updateData ={

&quot;\_id&quot;:&quot;visitors&quot;,

value: visitors

};

if(dbRev !==&quot;&quot;)

updateData[&quot;\_rev&quot;]= dbRev;

With the update hash table ready, we can insert the latest version into the database, using the [\&lt;database\&lt;.insert()](https://github.com/cloudant-labs/cloudant-nano#document-functions) function.

mydb.insert(updateData,

(err, body)=\&gt;{

If the insertion is successful, the response body includes the new revision value.

if(err ===undefined)

dbRev = body[&quot;rev&quot;];

These lines log database failures. The mechanism used for this is explained in later in this article.

else

log +=&quot;updateVisitors: &quot;+ err +&quot;\&lt;br\&gt;&quot;;

}

);

};

  The next few lines in the code read visitors when the application is started, using the [\&lt;database\&gt;.get()](https://github.com/cloudant-labs/cloudant-nano#document-functions) function.

// Read the visitors data structure.

mydb.get(&quot;visitors&quot;,(err, body)=\&gt;{

If we get a **404** error, it means there is no visitors data structure yet in the database. In this case, we create one and call updateVisitors(). This is the one case where the database.insert() function is called without a revision.

// No visitors yet, create it.

if(err !==null&amp;&amp; err.statusCode ===404){

visitors ={&quot;Test user&quot;:{arrived: Date.now().valueOf()}};

updateVisitors();

}else{

If there is a value, use it and keep the revision for when updateVisitors() needs it.

visitors = body.value;

dbRev = body[&quot;\_rev&quot;];

}

});

  The only function that directly changes visitor information after the application starts is setVisitor(). It needs to call updateVisitors() to save the change in the database.

varsetVisitor=(name, values)=\&gt;{

visitors[name]= values;

updateVisitors();

};

1.

### Time and date representation

There is one additional problem. Because the communication with Cloudant is text based, when writing to Cloudant Date objects are converted to their text representation, a string with the date, time, and time zone. Then, when the information is read back, they are treated as strings. This would be fine if we only wanted to display dates, but we also want the user to see how long each visit was.

To solve this problem, instead of storing a Date object in the visitors data structure and the database, we store the number of milliseconds since the beginning of the epoch (an arbitrary point in time, usually set on UNIX-derived systems to midnight on January 1, 1970, GMT). Storing milliseconds requires a few changes in the program:

First, every place where we get the current date needs to be Date.now().valueOf(). The valueOf() call turns the date object into the number of milliseconds since the beginning of the epoch. For example, in logout():

history.unshift({

arrived: oldRecord.arrived,

left: Date.now().valueOf()

});

The functions that display date and time stamps also need to change. To turn the time in milliseconds into a string, we create a new Date object with the time in milliseconds in one function, histEntryToRow():

// Given a history entry (arrived and left times), create a table row

// with that information

varhistEntryToRow=(entry)=\&gt;{

return`\&lt;tr\&gt;

\&lt;td\&gt;${new Date(entry.arrived)}\&lt;/td\&gt;

\&lt;td\&gt;${new Date(entry.left)}\&lt;/td\&gt;

\&lt;td\&gt;${tdiffToString(entry.left-entry.arrived)}\&lt;/td\&gt;

\&lt;/tr\&gt;`;

// The Date need to be new, otherwise we are just

// modifying the same object and all dates in

// the history table are the same.

};

There is one &quot;slight&quot; problem with the application. Every time that it is restarted it loses the visitor log. To solve this, we store the visitor log in a Cloudant database. The visitor name is the key, and the data (history and arrival time and date) is the value.

### Create the database

Follow these steps to create the database:

1. In the [IBM Cloud consoleIBM Cloud Dashboard](https://console.bluemix.net/dashboard/apps/?cm_sp=dw-bluemix-_-se-bluemix-self-posting-app-mean-stack-part1-_-article), click **Catalog** on the top left.
2. Click on **Databases** on the left navigation bar then click on **Cloudant**.

 ![](RackMultipart20210911-4-8gav30_html_64e1472f205b77f7.png)

Figure 35. IBM Cloud catalog

1. Name the service **visitor-log** and choose **&quot;**** Use both legacy credentials and IAM ****&quot;** under **Available authentication methods** and then finally click **Create**.

 ![](RackMultipart20210911-4-8gav30_html_aac00b5f0932b187.png)

Figure 36. Configuring Cloudant DB

1. When the service is created, click **Service credentials** in the left sidebar and then click the **New credential** button.

 ![](RackMultipart20210911-4-8gav30_html_61b929667d88b8d4.png)

Figure 37. Setting up Cloudant DB credentials

1. Name the new credential visitor-log and leave everything else as default. click Click **Add**.

![](RackMultipart20210911-4-8gav30_html_85718740f34150b5.png)

Figure 38. Setting up Cloudant DB credentials

1. In the credential list, click **View credentials**. Click the copy/duplicate icon to copy the credential and paste it to a text file.

 ![](RackMultipart20210911-4-8gav30_html_7139466cf9341514.png)

Figure 39. Cloudant DB credentials

1. In the left sidebar, click **Manage**. Then, click the **LAUNCH CLOUDANT DASHBOARD** button (you can also access it by using the credentials you just saved and accessing this link: https://\&lt; **Add your username here** \&gt;.cloudant.com/dashboard.html)

 ![](RackMultipart20210911-4-8gav30_html_b6457f75179e9ba5.png)

Figure 40. Cloudant dashboard

1. In the left sidebar, click the **Databases** icon.

 ![](RackMultipart20210911-4-8gav30_html_319dd643ebc73125.png)

Figure 41. Cloudant databases&#39; window

1. Then click **Create Database** in the upper right, name your database visitor-log and click **Create**.

![](RackMultipart20210911-4-8gav30_html_74554a091ffda5d4.png)

Figure 42. Creating a database

1. Go back to the application development environment and open the file **package.json**.
2. In the dependencies object, add a comma and then a line for the Cloudant package (version 1.7.x).

&quot;cloudant&quot;: &quot;1.7.x&quot;

 After you finish, your file will look like this:

 ![](RackMultipart20210911-4-8gav30_html_807e7e27f1e4992.png)

Figure 43. package.json

### Use the database

1. To use the database, replace **app.js** with [this code](https://github.com/qbzzt/bluemix/blob/master/security/201803/Visitor_Log/05-app.js). It uses almost the same data definitions and user interface, so it won&#39;t look different. But there is some additional code for integrating the database so if you now restart the application, the information will not be lost.

 The only thing you need to add before re-deploying the app is to add the cloudant Cloudant credentials you copied earlier intro this variable:

var cloudantCred = {
 \&lt;\&lt;
 redacted
 \&gt;\&gt;
 };

 Delete the part with \&lt;\&lt;\&gt;\&gt; and and paste your credentials, it should look like this:


 ![](RackMultipart20210911-4-8gav30_html_fbd2ff41c7547f8d.png)

Figure 44. Adding Cloudant credentials to the application

Go ahead and re-deploy the application. You will see some new test users and any new users will be added to your database.

1. This credential is to connect to the database management system (uses the url URL that you added in the cloudantCred variable), and then specifies which database you are going to use:

// Connect to the database

var cloudant = require(&quot;cloudant&quot;)(cloudantCred.url);

var mydb = cloudant.db.use(&quot;visitor-log&quot;);

1. There are two ways we can store the information in the database. One would be to put the entire visitors data structure in a single database entry (called document in Cloudant). The other is to have a separate document for each visitor name. For this introductory course, we will use the first method. It is less efficient, but [it will work for up to 1 MB](https://console.bluemix.net/docs/services/Cloudant/api/document.html#documents). The major advantage of this approach is that we can use the application logic developed previously with almost no change. We can continue to keep the visitors data structure as a variable.


2. The same Cloudant database could be used by multiple applications at the same time. To avoid one application&#39;s interference with another, it uses a revision system. Every document has a \_rev value with the current revision. When you update a document, you provide the revision you&#39;re updating. If it changed from the time you read it, the revision is different causing the update to fail—this requires us to have a variable to hold the current revision.

var dbRev = &quot;&quot;;


3. This function updates the visitor log on the database.

var updateVisitors = () =\&gt; {

 The data to update always includes \_id, the key, and the actual value. It usually also includes \_rev, the revision. The exception is when creating a new entry.

var updateData = {

        &quot;\_id&quot;: &quot;visitors&quot;,

        value: visitors

};

if (dbRev !== &quot;&quot;)

    updateData[&quot;\_rev&quot;] = dbRev;


With the update hash table ready, we can insert the latest version into the database, using the [\&lt;database\&gt;.insert\&lt;database\&gt;.insert()](https://github.com/cloudant-labs/cloudant-nano#document-functions) function.

mydb.insert(updateData,

    (err, body) =\&gt; {

If the insertion is successful, the response body includes the new revision value.

if (err === undefined)

dbRev = body[&quot;rev&quot;];

These lines log database failures. The mechanism used for this is explained in later in this article.

            else

                log += &quot;updateVisitors: &quot; + err + &quot;\&lt;br\&gt;&quot;;

        }

    );

};

1. The next few lines in the code read visitors when the application is started, using the [\&lt;database\&gt;.get\&lt;database\&gt;.get()](https://github.com/cloudant-labs/cloudant-nano#document-functions) function.

// Read the visitors data structure.

mydb.get(&quot;visitors&quot;, (err, body) =\&gt; {

If we get a **404** error, it means there is no visitors data structure yet in the database. In this case, we create one and call updateVisitors(). This is the one case where the database.insert() function is called without a revision.

// No visitors yet, create it.

if (err !== null &amp;&amp; err.statusCode === 404) {

    visitors = {&quot;Test user&quot;: {arrived: Date.now().valueOf()}};

    updateVisitors();

} else {

If there is a value, use it and keep the revision for when updateVisitors() needs it.

        visitors = body.value;

        dbRev = body[&quot;\_rev&quot;];

    }

});

1. The only function that directly changes visitor information after the application starts is setVisitor(). It needs to call updateVisitors() to save the change in the database.

var setVisitor = (name, values) =\&gt; {

    visitors[name] = values;

    updateVisitors();

};

### Time and date representation

There is one additional problem. Because the communication with Cloudant is text based, when writing to Cloudant Date objects are converted to their text representation, a string with the date, time, and time zone. Then, when the information is read back, they are treated as strings. This would be fine if we only wanted to display dates, but we also want the user to see how long each visit was.

To solve this problem, instead of storing a Date object in the visitors data structure and the database, we store the number of milliseconds since the beginning of the epoch (an arbitrary point in time, usually set on UNIX-derived systems to midnight on January 1, 1970, GMT). Storing milliseconds requires a few changes in the program:

First, every place where we get the current date needs to be Date.now().valueOf(). The valueOf() call turns the date object into the number of milliseconds since the beginning of the epoch. For example, in logout():

history.unshift({

    arrived: oldRecord.arrived,

    left: Date.now().valueOf()

});

The functions that display date and time stamps also need to change. To turn the time in milliseconds into a string, we create a new Date object with the time in milliseconds in one function, histEntryToRow():

// Given a history entry (arrived and left times), create a table row

// with that information

var histEntryToRow = (entry) =\&gt; {

    return `\&lt;tr\&gt;

        \&lt;td\&gt;${new Date(entry.arrived)}\&lt;/td\&gt;

        \&lt;td\&gt;${new Date(entry.left)}\&lt;/td\&gt;

        \&lt;td\&gt;${tdiffToString(entry.left-entry.arrived)}\&lt;/td\&gt;

        \&lt;/tr\&gt;`;

        // The Date need to be new, otherwise we are just

// modifying the same object and all dates in

        // the history table are the same.

};

## Logging for debug purposes

While developing this application, I needed to see why database updates did not work sometimes. To see why some database updates faileddo that, I created a log string and appended to it every time an update failed. This technique can also be useful in your web applications (make sure to disable it or require a secret before you have production data).

need to be new, otherwise we are just

var log = &quot;&quot;;



var updateVisitors = () =\&gt; {

...

    mydb.insert(updateData,

        (err, body) =\&gt; {

            if (err === undefined)

                dbRev = body[&quot;rev&quot;];

            else

When we add to the log, append a \&lt;br/\&gt;. This string will be retrieved by a browser, which will interpret it as HTML by default.

log += &quot;updateVisitors: &quot; + err + &quot;\&lt;br\&gt;&quot;;

        }

    );

};

To access the log, go to the /log path:

app.get(&quot;/log&quot;, (req, res) =\&gt; {

    res.send(log);

});




