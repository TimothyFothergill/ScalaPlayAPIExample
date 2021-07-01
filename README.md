# ScalaPlayAPIExample 

My first attempt at writing a full Scala Play project, from creation using `SBT` through to deployment.


## My Learning Process
### Getting Started

Using IntelliJ IDEA as my IDE of choice.\
Following the documentation on https://playframework.com, ran the following command:\
`sbt new playframework/play-scala-seed.g8`

This creates a new Scala Play project using SBT (Scala Build Tool).\
Created git repository and pushed initial build to `main` branch. \
`git checkout` to create a new branch and began the initial build.

![Fig-1 - Shows the sbt play framework default project running locally](scalaplayapiexample-images-for-readme/fig%201%20-%20Welcome%20to%20Play.png)

### Adding another webpage

Adding another webpage was as simple as creating a new HTML file using the template provided.

![Fig-2 - Showing another html file made to act as another webpage for the site.](scalaplayapiexample-images-for-readme/fig%202%20-%20Adding%20another%20html%20page.png)

After this was added, I added in a method in the HomeController:

![Fig-3 - New method added into HomeController, follows the logic of the default.](scalaplayapiexample-images-for-readme/fig%203%20-%20Adding%20controller%20method%20for%20another%20html%20page.png)

Finally I added a route in `conf/routes`. At this point in the application, my conf/routes looked like this:
```
# An example controller showing a sample home page
GET     /                           controllers.HomeController.index()
GET     /our-services               controllers.HomeController.ourservices()
```
