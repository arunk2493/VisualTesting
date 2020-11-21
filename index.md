## Visual Testing

In the current testing world, Visual Testing is one of the most buzz word technology among the QAs in the industry. What is Visual Testing????

- The visual aspects of the application’s user interface seems appropriate to the user.
- Correct data and content are getting displayed at the application’s front end.
- Verifying and Validating the visual appearance of each element that is present in the UI.

The above 3 aspects are very important for an application that needs to be a visual treat for the users.

## What,Who,Where,When & How - Visual Regression Testing

- WHAT is Visual Regression Testing?
 
 A technique which performs front end / User Interface elements testing by taking screenshots of webpages / UI components and compare them with the original      images(baseline screenshots)

- WHO are responsible for performing the testing?
  
  Quality Analyst / UI developers

- WHERE the testing occurs?
 
 As we are going to use StoryBook so the testing occurs in an isolated environment without worrying about the app specific dependencies and requirements
 
- WHEN the testing can be conducted?
 
 During any new UI component development / Changes
  
- HOW can we do the testing?
  
  Comparing the screenshots with the current and the latest build by manually or using some tools
  
  ## A Quick look of how Visual Testing using automation works
   
   - Run the test code against the stable build of the application and capture the screenshot (Base Line Images)
   - Now let's consider any new UI change has occured, 
      
      For example let's consider a Fashion Retail Application. In the stable build if we apply any filter criteria the result page is loaded correctly. But in the next build there was UI alignment changes made and we don't know how it will reflected until unless we push the changes to the dev / localhost environment. So to avoid such confusions before deploying the UI part to the dev / test environment we can write an automation code to compare the prevoius build application UI elements with the current build's UI element and see if any major changes has happened.
      
      If there are some changes in the DOM content then either we can accept those changes and push the changes to our repository or else we can reject the changes and again work on those part and make it better
  
  ![Visual Testing](https://qanish.files.wordpress.com/2019/02/screenshot-difference-e1545051723765-1.png?w=1312&h=600&crop=1)

