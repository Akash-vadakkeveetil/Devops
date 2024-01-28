<h1 align="center">What are Build and Package Manager Tools? ⚙️</h1>
<hr>

  
To deploy the application on a production server, the developer needs to package the application into a single movable file, known as an ==artifact==. This involves the process of packaging, which essentially means building the code along with its dependencies. Once the packaging is complete, the resulting artifact contains the entire application code and its required dependencies. This consolidated file can then be easily transported and deployed on the production server for seamless execution. In essence, packaging is the crucial step in preparing the application for deployment, ensuring that it can be efficiently moved and run on the designated server.

### Where do we store these artifacts ??

The place where we store the artifacts is known as the Artifact repository.
Some of them are : JFrog ARTIFACTORY , NEXUS 


The development process involves compiling the application code, consolidating it from hundreds of files into a single executable file. Subsequently, this compiled artifact is compressed to reduce its size, making it more manageable. The compressed artifact is then stored in a designated storage system, allowing for easy retrieval and deployment.

This stored artifact serves as a reliable backup, facilitating multiple deployment instances and safeguarding against potential issues. Before deployment, thorough testing is essential to ensure the application functions as intended. Finally, the compressed and tested artifact is deployed to the production server, where it can run efficiently in a live environment. This comprehensive process ensures a streamlined and reliable approach to managing, deploying, and maintaining the application in a production setting


### What kind of file is the artifact?

In the context of Java applications, it could be a JAR (Java Archive) file or a WAR (Web Archive) file for web applications. These include whole code + the dependencies for other frameworks and libraries such as Spring framework, datetime libraries, PDF processing libraries.