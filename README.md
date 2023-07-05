
[![Build Status](https://app.travis-ci.com/aisabel/SwaggerPetStore-Postman.svg?branch=main)](https://app.travis-ci.com/aisabel/SwaggerPetStore-Postman.svg?branch=main)


<h2>Business Requirement:</h2>
<p align="justified">Create automated tests to cover at least the CRUD (create, read, update, delete) operations on a pet store website</p>

<h2>TestFramework Description:</h2>
<p align="justified">This test suite was designed to meet business requirements by createing automated test based on a swagger api: petstore.swagger.io</br>
 Postman is an API client that makes it easy for developers to create, share, test and document APIs. This is done by allowing users to create and save simple and complex HTTP/s requests, as well as read their responses. </br>This test suite is configured to be continuosly integrated in <a href="https://app.travis-ci.com/github/aisabel/SwaggerPetStore-Postman/builds">Travis</a> for a fast pace development environment.</p>
 
 <h2>Specifications:</h2>
<ul>
  <li><a href="https://www.postman.com/product/what-is-postman>*Postman Version 9.25.1</a></li>
  <li><a href="https://nodejs.org/dist/v16.16.0/node-v16.16.0-x64.msi">*Node js LTS version 16.16</a></li>
   <li><a href="https://www.npmjs.com/package/newman">*Newman 5.3.2</a></li>
  <li><a href="https://github.com/DannyDainton/newman-reporter-htmlextra">*html reporter extra </a></li>
  <li><a href="https://docs.travis-ci.com/user/tutorial/">*Travis CI </a></li>
   
</ul>

<h2>TestingFramework Structure:</h2>
In order to provide a clear functional framework, the structure has been settup as below:</br>
</br>

<ul>
|--results</br>
|--tests:</br>
<ul>
 <li>PetStoreEnv.postman_collection.json = environment defined to run collection</li>
 <li>SwaggerPetStore.postman_collection.json = postman collection</li>
</ul>
</ul>


<h2>Install</h2>
<p>Postman application is open source software, a Javascript application designed to load test functional behavior. Postman's features simplify each step of building an API and streamline collaboration so you can create better APIs—faster. The tool can be downloaded at: https://www.postman.com/downloads/</br>
Postman test can be run from command line using node.js https://nodejs.org/es/
</p>

<h2>Run Tests: </h2>
<h3>How to run tests locally using Postman</h3>
<ul>
  <li>Install Postman</li>
  <li>Double click to open postman</li>
  <li>In the top menu go to File > Import</li>
  <li>Locate in your local machine the file with the postman_collection extension </li>
  <li>Click on the gear in the right top "manage environments" and choose from your local machine the file with the environent extension</li>
  <li>Click on "Import" button</li>
  <li>There are two ways to send request: The first one is click on each request and then click button "send". The other one is to click button in the top menu "Runner"</li>
  <li>The first one is click on each request and then click button "send".</li>
  <li>The other one is to click button in the top menu "Runner", select the collection to run and the environment to be used and click button "Start Run". Within this option the number of iterations can be set up manually so the runner will be exceuted "n" times. This option also allows to add delays between each request.</li>
 </ul>
<h3>How to run tests from the command line</h3>
<ul>
  <li>To run the testplan from the command line you need to open a command prompt of Node.js</li>
  <li>Traverse locally until folder where postman test are located</li>
  <li>Run the command: newman run with the following parameters: </il>
    <li>Parameters:
<ol>- Path to the collection name</ol>
<ol>- folder name to run (if applies)</ol>
<ol>- environment to use</ol>
<ol>- the last part is the one where you will store the report formatter (the formatter is located in this repo for your convenience)
finally the last part has the name of the html file where you will find the results of the test.</ol>
</li>
<li>Example:  newman run C:\git\Projects\PetStore.postman_collection.json -e C:\git\Projects\environments\PetStore.postman_environment.json --delay-request 2000 --reporters cli,html --reporter-html-export PostmanResult.html</li>
<li><b>Note:</b> the postman files must have the extension .json in order to be used with newman, otherwise will not be recognized</li>
</ul>
    
<h2>External references: </h2>
<ul>
<li><a href="https://learning.postman.com/docs/postman/collection-runs/command-line-integration-with-newman/">Command line integration with newman</a></li>
<li><a href="https://www.npmjs.com/package/newman-reporter-htmlextra">Newman reporter</a></li>
<li><a href="https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions">Github Actions</a></li>
</ul>

   
