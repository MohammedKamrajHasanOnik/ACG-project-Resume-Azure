<h1>ACG-project-Resume-Azure(with Blob Storage, Functions, CosmosDB, and Github Actions)</h1>


<h2>(A Cloud Guru youtube video followed as guide)</h2>

<h2>Description</h2>
This project is a guide of how I built my resume on Azure, the core bones solution would be inside of the Blob Storage, which will hold my static website i.e. Resume. In that website we will be utilizing HTML,CSS and JavaScript. The javascript will be utilzied to implement a visitor counter, which will be used to display the information but to importantly call an API, which I am going to  apply with an Azure function. Further to insinuate the azure function is going to intermingle with Azure Cosmos DB. This is the database service I will be using to store the visitor counter information. I am also going to use Azure CDN to enable features like HTTPS and custom domain support for my static site. That is deployed on Azure blob storage. Finally, for all my CI/CD tooling, I am going to use GitHub.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Azure Functions Core Tools</b> 
- <b>.NET Core 3.1 SDK</b>
- <b>Azure Cli</b>
- <b>C# Extension</b>

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
<h2 align="center">Program guide</h2>

<p align="center">
<b>The network diagram as shown I will be utilizing for the project</b> <br/>
<img src="https://i.imgur.com/ceuZrI3.jpg"/>
<br />
<br />
<br />
<h3> Section 1 Building the frontend
<b>Creating Server 2019, assigning it 2048mb memory ram approx 2gb and 3 processors VM</b> <br/>
<img src="https://i.imgur.com/nqjMOCy.jpg"/>
<br />
<br />
<br/>
