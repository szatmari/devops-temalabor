# SpringBoot application project generation and testing


- Based on the https://spring.io/quickstart tutorial, use the https://start.spring.io/ project generator to generate a new Web-enabled SpringBoot project
- Setup an IDE for your project (VSCode, IntelliJ or any of your choice)
- Add some HTTP GET Mapping definitions to the Application class to specify an example HTTP response
  - Add Java import specifications
  - Add the @RestController annotation to the class
  - Add function with a @GetMapping annotation and specify the behaviour
- Test the HTTP GET Parameter management
- Using the bootBuildImage Gradle task build a docker image for your project
  - `gradle bootBuildImage`
- Test the docker image, start it and using a port mapping publish the default port 8080 to your host interface and check the content using a browser
  - `docker run -it -p 8080:8080 *image-name*`
  - http://localhost:8080/*your-get-endpoint*


