# SwaggerPetStore-Postman
[![Build Status](https://app.travis-ci.com/aisabel/SwaggerPetStore-Postman.svg?branch=main)](https://app.travis-ci.com/aisabel/SwaggerPetStore-Postman.svg?branch=main)


<h2>Business Requirement:</h2>
<p align="justified">Create automated tests to cover at least the CRUD (create, read, update, delete) operations on a pet store website</p>

<h2>TestFramework Description:</h2>
<p align="justified">This test suite was designed to meet business requirements by createing automated test based on a swagger api: petstore.swagger.io</br>
 Postman is an API client that makes it easy for developers to create, share, test and document APIs. This is done by allowing users to create and save simple and complex HTTP/s requests, as well as read their responses. This test suite is configured to be continuosly integrated in <a href="https://app.travis-ci.com/github/aisabel/SwaggerPetStore-Postman/builds">Travis</a> for a fast pace development environment.</p>
 
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
|--SwaggerPetStore/reportst</br>
|--SwaggerPetStore/tests:</br>
<ul>
 <li>PetStoreEnv.postman_collection.json = environment defined to run collection</li>
 <li>SwaggerPetStore.postman_collection.json = postman collection</li>
</ul>
</ul>

  
<h2>How to run tests: (Documentation steps in progress...)</h2>
   
