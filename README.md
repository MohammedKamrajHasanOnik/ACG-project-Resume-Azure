<h1>ACG-project-Resume-Azure(with Blob Storage, Functions, CosmosDB, and Github Actions)</h1>


<h2>(A Cloud Guru youtube video followed as guide -https://www.youtube.com/watch?v=ieYrBWmkfno)</h2>

<h2>Description</h2>
This project is a guide of how I built my resume on Azure, the core bones solution would be inside of the Blob Storage, which will hold my static website i.e. Resume. In that website we will be utilizing HTML,CSS and JavaScript. The javascript will be utilzied to implement a visitor counter, which will be used to display the information but to importantly call an API, which I am going to  apply with an Azure function. Further to insinuate the azure function is going to intermingle with Azure Cosmos DB. 
(This is the database service I will be using to store the visitor counter information. I am also going to use Azure CDN to enable features like HTTPS and custom domain support for my static site. That is deployed on Azure blob storage. Finally, for all my CI/CD tooling, I am going to use GitHub)- Wanted to do these steps but could not due to technical difficulties, in applications, programs, coding etc.
<br/>

<h2>Languages and Utilities Used</h2>

- <b>Azure Functions Core Tools</b> 
- <b>.NET Core 3.1 SDK</b>
- <b>Azure Cli</b>
- <b>C# Extension</b>
- <b>Javascript</b>
- <b>HTML</b>

<h2>Environments Used </h2>

- <b>Azure Account</b>
- <b>Visual Studio Code</b>
- <b>Windows 10</b> 

<h2>Links to programs and scripts required</h2>

- <b>Git Hub:</b> https://github.com/
- <b>Azure Account:</b> https://azure.microsoft.com/en-us/free
- <b>Azure CLI:</b> https://learn.microsoft.com/en-us/cli/azure/install-azure-cli
- <b>.NET Core 3.1 LTS:</b> https://dotnet.microsoft.com/en-us/download/dotnet/3.1
- <b>Azure Functions Core Tools:</b>https://learn.microsoft.com/en-us/azure/azure-functions/functions-run-local?tabs=macos%2Cisolated-process%2Cnode-v4%2Cpython-v2%2Chttp-trigger%2Ccontainer-apps&pivots=programming-language-csharp#install-the-azure-functions-core-tools
- <b>Visual Studio Code:</b> https://code.visualstudio.com/
- <b>Visual Code Extensions:</b> https://code.visualstudio.com/docs/introvideos/extend
- <b>Azure Functions Extensions:</b> https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurefunctions
- <b>C# Extension:</b> https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp
- <b>Azure Storage Extension:</b> https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurestorage
- <b>git application:</b> https://git-scm.com/download/win
<br/>
<br/>
<br/>
<h2 align="center">Program guide</h2>
<p align="center">
<b>The network diagram as shown I will be utilizing for the project</b> <br/>
<img src="https://i.imgur.com/8NBSClG.jpeg"/>
<br/>
<br/>
<br/>
<h3> Section 1 Building the frontend</h3>
<br/>
<br/>
<h4>ssh private and public key generated using command prompt</h4>
<p align="left"> 
<img src="https://i.imgur.com/xJ8MjIP.jpeg"/>
<br/>
<br/>
<br/>
<h4>Add new SSH key public key opened in notepad</h4>
<p align="left"> 
<img src="https://i.imgur.com/AmlB0Wi.jpeg"/>
<br/>
<br/>
<br/>
<h4>pressed add new key confirmation of ssh publick key added</h4>
<p align="left">  
<img src="https://i.imgur.com/cS5oMMA.jpeg"/>
<br/>
<br/>
<br/>
<h4>git repository cloned into ACG-Project-Resume-Azure</h4>
<p align="left"> 
<img src="https://i.imgur.com/NSNfwHf.jpeg"/>
<br/>
<br/>
<br/>
<h4>ACloudGuru-Resources acg-project-azure-resume-starter git repository cloned</h4>
<p align="left">  
<img src="https://i.imgur.com/XwIvZHp.jpeg"/>
<br/>
<br/>
<br/>
<h4>Copied backend and frontend acg project azure resume starter to my acg project resume azure folder</h4>
<p align="left"> 
<img src="https://i.imgur.com/DXfFagj.jpeg"/>
<br/>
<br/>
<br/>
<h4>making changes to webpage HTML document index.html, document links to my personal social media links</h4>
<p align="left"> 
<img src="https://i.imgur.com/E9nk0jF.jpeg"/>
<br/>
<br/>
<br/>
<h4>Making changes to index.html file html document changes to education schools section</h4>
<p align="left"> 
<img src="https://i.imgur.com/VylSpY8.jpeg"/>
<br/>
<br/>
<br/>
<h4>Making changes to index.html file certifications section</h4>
<p align="left">  
<img src="https://i.imgur.com/8ivmK84.jpeg"/>
<br/>
<br/>
<br/>
<h4>Making changes to index.html work section</h4>
<p align="left">  
<img src="https://i.imgur.com/AuZA3h7.jpeg"/>
<br/>
<br/>
<br/>
<h4>Javascript code for the getvisit count method, function and array utilized</h4>
<p align="left">  
<img src="https://i.imgur.com/I0E9WBF.jpeg"/>
<br/>
<br/>
<br/>
<h4>git commit updates, to structure, created main.js file</h4>
<p align="left">  
<img src="https://i.imgur.com/vFP4RqH.jpeg"/>
<br/>
<br/>
<br/>
<h4>git push done enumurating objects to my github acg Rezume Azure repoistory</h4>
<p align="left">  
<img src="https://i.imgur.com/C1Dq8hK.jpeg"/>
<br/>
<br/>
<br/>
<h4>Back-End</h4>
<br/>
<br/>
<br/>
<h4>Creating CosmoDB for NoSQL, subscription name, resource group, location and serverless added and assigned</h4> 
<p align="left">  
<img src="https://i.imgur.com/otCxkSl.jpeg"/>
<br/>
<br/>
<br/>
<h4>Creating new ResumeAzure Database</h4>
<p align="left">  
<img src="https://i.imgur.com/A3fUimN.jpeg"/>
<br/>
<br/>
<br/>
<h4>Creating new container in ResumeAzure database</h4>
<p align="left">  
<img src="https://i.imgur.com/UarNOw8.jpeg"/>
<br/>
<br/>
<br/>
<h4>Meta data inside of our items and id count</h4>
<p align="left"> 
<img src="https://i.imgur.com/k5N7DcR.jpeg"/>
<br/>
<br/>
<br/>
<h4>get resume counter.cs created from backend api added HTTP Aspnet core, C#, .Net8 etc</h4>
<p align="left">  
<img src="https://i.imgur.com/dN36GLa.jpeg"/>
<br/>
<br/>
<br/>
<h4>My resume online html webpage file opened</h4>
<p align="left">  
<img src="https://i.imgur.com/4NiMk4z.jpeg"/>
<br/>
<br/>
<br/>
<h4>My resume about me, profile picture, universities, education, work, certifications, and social link </h4>
<p align="left">  
<img src="https://i.imgur.com/56ooVcA.jpeg"/>
<br/>
<br/>
<br/>
-<b> This project could not be fully completed due to Net error, driver packages, and outdated coding, however I fully completed the front end and back end, as well as editing the html document. I searched youtube for a recent walkthrough could not find a recent walkthrough guide. 
