# SpringBoot application project generation and testing


- Based on the https://spring.io/quickstart tutorial, use the https://start.spring.io/ project generator to generate a new Web-enabled SpringBoot project
  - Prefer to use a Gradle project
  - Add the Spring Web dependency
  - Set the metadata on your choice
- Test the build of the project using CLI
  - E.g. using the `gradle bootJar` task.
- Setup an IDE for your project (VSCode, IntelliJ or any of your choice)
- Add some HTTP GET Mapping definitions to the Application class to specify an example HTTP response
  - Add Java import specifications
  - Add the @RestController annotation to the class
  - Add function with a @GetMapping annotation and specify the behaviour
- Test the HTTP GET Parameter management
- Execute the project on your local machine
  - `gradle bootRun`
  - `curl localhost:8080/*your-get-endpoint*`
  - http://localhost:8080/*your-get-endpoint*
- Using the bootBuildImage Gradle task build a docker image for your project
  - `gradle bootBuildImage`
- Test the docker image, start it and using a port mapping publish the default port 8080 to your host interface and check the content using a browser
  - `docker run -it -p 8080:8080 *image-name*`
  - http://localhost:8080/*your-get-endpoint*


## References

- Docker overview: https://docker-curriculum.com/#introduction
- ReteLab1 education material: https://ftsrg.mit.bme.hu/rete-lab-lecture-notes/retelab1-lab4-deployment.html
- DevOps course material - Docker: https://inf.mit.bme.hu/sites/default/files/materials/category/kateg%C3%B3ria/oktat%C3%A1s/v%C3%A1laszthat%C3%B3-t%C3%A1rgyak/devops/19/05_Docker.pptx
- DevOps course material - Build: https://inf.mit.bme.hu/sites/default/files/materials/category/kateg%C3%B3ria/oktat%C3%A1s/v%C3%A1laszthat%C3%B3-t%C3%A1rgyak/devops/19/02_Verzi%C3%B3kezel%C3%A9s-Ford%C3%ADt%C3%A1s.pptx

