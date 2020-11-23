## Visual Testing

In the current testing world, Visual Testing is one of the most buzz word technology among the QAs in the industry. What is Visual Testing????

- The visual aspects of the application’s user interface seems appropriate to the user.
- Correct data and content are getting displayed at the application’s front end.
- Verifying and Validating the visual appearance of each element that is present in the UI.

The above 3 aspects are very important for an application that needs to be a visual treat for the users.

## What,Who,Where,When & How - Visual Regression Testing

  ## WHAT is Visual Regression Testing?
 
   A technique which performs front end / User Interface elements testing by taking screenshots of webpages / UI components and compare them with the original         images(baseline screenshots)

  ## WHO are responsible for performing the testing?
  
   Quality Analyst / UI developers

  ## WHERE the testing occurs?
 
   As we are going to use StoryBook so the testing occurs in an isolated environment without worrying about the app specific dependencies and requirements
 
  ## WHEN the testing can be conducted?
 
   During any new UI component development / Changes
  
  ## HOW can we do the testing?
  
   Comparing the screenshots with the current and the latest build by manually or using some tools
  
  ## Automation Tools for Visual Testing
  
   There are many tools for performing the visual testing. But the most poweful, interactive tools for performing this testing are,
    
    1. Applitools
    2. Chromatic
    3. Percy
   
   Both these tools are licensed, unique and they provide their own features including the dashboard for each project and account, running the code against the git commit(Chromatic), integrating with CI and executing the code upon multiple platforms,browsers(Applitools)
   
   Applitools supports almost all the programming languages whereas Chromatic supports all the UI languages integrated with StoryBook. 
   
   - To know about [StoryBook](https://storybook.js.org/)
   - To know about [Applitools](https://applitools.com/)
   - To know about [Chromatic](https://www.chromatic.com/)
   
  ## Ways how visual testing can be done in automation
   
   - The first way is we can run our test scripts across UAT and Test environments and verify the visual aspects after any change in the UI
   - Another way is we can run our test scripts across the git commits i.e, the last commit and current commit.
   
   So, from this we understood that the visual testing can be done across the environments and also across the last and the current commit in the git.
  
  ## A Quick look of how Visual Testing using automation works with the First Way
   
   - Run the test code against the stable build of the application and capture the screenshot (Base Line Images)
   - Now let's consider any new UI change has occured, 
      
      For example let's consider a Fashion Retail Application. In the stable build if we apply any filter criteria the result page alignment is loaded correctly. But in the current build there was some UI alignment changes made and we don't know how it will reflected until unless we push the changes to the dev / localhost environment.
      So to avoid such confusions before deploying the UI part to the dev / test environment we can write an automation code with some of the visual testing tools to compare the stable build UI elements with the current build's UI element and see if any major changes has happened.
      
      If there are some changes in the DOM content then either we can accept those changes and push the changes to our repository or else we can reject the changes and again work on those part and make it better
      
      - Compare the stable build UI screenshot(Baseline Screenshot) with the current build screenshot(Actual UI screenshot)
      
  
  ![Visual Testing](https://qanish.files.wordpress.com/2019/02/screenshot-difference-e1545051723765-1.png?w=1312&h=600&crop=1)
  
  So from the above scenario it's clear that we can able to visually compare the UI of an application with stable and current builds by capturing the screenshots and verifying with the DOM content.
  
  _Here stable and current build refers to UAT and Dev environment respectively._
  
  This blog is purely based upon my learnings, if anything needs to be added, always open to accept feedbacks.
  
  Will try post some code based blog with Applitools and Chromatic in my future posts.
  
  ## Learn..Educate..and Shine!!
  
  

