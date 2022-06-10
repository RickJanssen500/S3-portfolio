## Learning outcomes
## 1 You design and build user-friendly, full-stack web applications. IP and GP   
   The design and tech choises for my project can be found [here](https://github.com/RickJanssen500/S3-portfolio/blob/main/individual%20project.md#individual-project).   
      
   ### backend   
   In my backend I have created 2 different microservices.   
   A microservice for making orders and a microservice for picking orders.   
   The microservices are both written in C#.   
   The only difference between them is that the order-api was made in .net 5 and the picking-api in .net 6.   
   In this I noticed little difference from creating the microservices.
   
   | ![image](https://user-images.githubusercontent.com/84378377/172845739-b77359cb-8732-4d01-ba10-76b762d333fa.png) | 
   | :--: |
   | _backend controller_ |     
      
   Above is a screenshot from the order controller of the order-api.   
   The 2 functions you see are the functions to add a product and to submit the order.   
   Because they are post methods, they only return a status code.   
   The status code that is returned is determined by the boolean that the BLL function returns back to the controller.   
      
   | ![image](https://user-images.githubusercontent.com/84378377/172845968-02233451-fc2b-4d2f-b6bf-d84b7eb2d164.png) | 
   | :--: |
   | _ Order backend swagger_ |     
      
   Here is a screenshot of the order-api.   
   The api calls are placed in 2 categories.   
   one for retrieving product information and one for retrieving and placing order information.   
   When placing an order, you do not need to change product information Therefore, there are no calls for this.      
      
   | ![image](https://user-images.githubusercontent.com/84378377/173013736-eefbf922-bf49-4515-af7a-329a6482597d.png) | 
   | :--: |
   | _Picking backend swagger_ | 
     
   Here is a screenshot of the picking-api.   
   The api calls are placed in 2 categories.   
   one for retrieving and changing  order-product information and one for retrieving and changing order information.   
      
   | ![image](https://user-images.githubusercontent.com/84378377/172846162-cabd9375-4638-4bd1-b238-e67f501ef3fd.png) | 
   | :--: |
   | _backend swagger call_ |   
      
   When calling an api-call, certain data must be provided.   
   For example, the product id and the user id must be given in the delete call seen above.   
   Thus the api knows from which user it should remove which product from the shopping cart.
      
   ### frontend   
   I have created my webshop frontend with javascripframework Vue.   
   Here you can see all the products and add them to your shopping cart.   
   Here you can also see how many products you have in your cart and navigate to your cart.
      
   | ![image](https://user-images.githubusercontent.com/84378377/172843957-fe8b2189-88da-4736-8c62-2331b9d80b15.png) | 
   | :--: |
   | _Mainview Vue_ |       
      
   The vue pages are made up of components.   
   Below you can see all the components that the frontend uses.
      
   | ![image](https://user-images.githubusercontent.com/84378377/172845158-b6f3c5fe-84c4-4978-8ea4-362846755362.png) | 
   | :--: |
   | _Vue component_ |   
      
   The "GetProducts", "SmallProduct" and "ProductAmount" are used for the home page.   
   The "GetProducts" contains all products, which are displayed by using "SmallProduct".   
   The "SmallProduct" component contains the "ProductAmount" component that allows the user to add a product to the shopping cart.   
   The "Cart", "CartItem" and "Complete" are used to view and complete the order.     
   The "Cart" contains all "CartItem" components.   
   The "Complete" component is loaded when a user wants to place an order.   
      
      
   For the orderpicking part of my project, I created a Xamarin mobile app as a second frontend.   
   The app can pick orders and shows notification and errors.   
      
   Below is the screen where the user can choose which order to pick.   
   For each order you see the order id and the date and time when the order will be collected.   
      
   | <img src="https://user-images.githubusercontent.com/84378377/172945933-3fe0b734-1758-48af-b085-4878e8695665.png" alt="image" width="250" height="490"/> | 
   | :--: |
   | _Orderview_ |      
      
   The screen below shows the notification that the app gives when there are no more orders to be collected.
      
   | <img src="https://user-images.githubusercontent.com/84378377/172946017-a06fd815-435d-486d-8b1f-3144060ab924.png" alt="image" width="250" height="490"/> | 
   | :--: |
   | _No order message_ |     
      
   The app can also display several errors. For example, if something goes wrong with making the api call or if the device has no internet.   
   The screen below shows the error that the app gives when you have no internet.
   
   | <img src="https://user-images.githubusercontent.com/84378377/172945902-299726fc-9e08-42f1-bb21-6df1ce4acea3.png" alt="image" width="250" height="490"/> | 
   | :--: |
   | _No internet error_ |    
      
      
## 2 You use software tooling and methodology that continuously monitors and improve the software quality during software development. IP only
   To ensure the quality of my code, I use testing.
   These tests show that the code does what it is supposed to do. The moment I change the code so that it no longer functions as it should,
   I see this immediately in the tests because the test fails in such a case.
   Because the tests have a clear name, I immediately know which function no longer works and for what reason it fails.
   For instance, the name of the test contains the name of the function and what of the function is being tested.
   So you can see in the picture below that the name of the test refers to finding a product and 
   the part it tests is the reaction that the api gives if there is no product with the given ID.
   | ![image](https://user-images.githubusercontent.com/84378377/171639679-8323b1fe-aa04-4682-a7bb-668a67192b11.png) | 
   | :--: |
   | _Test name for failed GetByID test_ |  
   
   Besides the clear naming of the tests, I also use several different types of tests.
   The 2 types of testing I use are unit testing and endpoint testing.
   The unit tests the functions from my business logic layer(BLL).
   The endpoint tests tests whether the api provides the right response codes and returns the right values.
   The values that the api returns are usually smaller objects than the BLL gives to the controller.
   This is because it is unnecessary to send extra data to the front-end that is not used anyway.
   The endpoint tests therefore do not only look at whether the correct status code is given but also whether the object returned by the bll is
   properly converted into the return object for the frontend.
   In total, I have 20 tests, of which 12 unit tests and 8 endpoint tests.
   | ![image](https://user-images.githubusercontent.com/84378377/171641657-79c7d941-599e-43eb-b953-5839f34c560e.png) | 
   | :--: |
   | _All tests_ |  
   
   All tests are structured in the same way using the 3 A's.
   Arrange, Act and Assert.
   At Arrange, I am going to create everything that the test needs to run.
   I create an in-memory database so that the test results are not influenced by an external database.
   Also, each test gets its own in-memory database to avoid database conflicts between different tests.
   With arrange, I also create all the necessary objects and variables to run the function.
   At Act, I execute the function and store the results of the function in variables.
   At Assert, I check whether the result given by the function corresponds to the expected result.
   Below is an example of a unit test and an end point test where you can clearly see that they have the same structure.
    | ![image](https://user-images.githubusercontent.com/84378377/171642574-652f7a71-d3df-4717-b48b-860bdf5acaeb.png) | 
   | :--: |
   | _Unit test_ |  
   
   | ![image](https://user-images.githubusercontent.com/84378377/171642266-51cac506-b028-4a42-a736-15fbaeb74b29.png) | 
   | :--: |
   | _Endpoint test_ |  
      
   To make sure my code quality is good I use Sonar Cload code scan to achieve this.   
   So that I know immediately which code smells are there.   
   | ![image](https://user-images.githubusercontent.com/84378377/172839466-652290f3-a9fa-4ea0-b244-b76e56ce1936.png) | 
   | :--: |
   | _Sonar Cload dashboard_ | 
   
## 4 You design and implement a (semi)automated software release process that matches the needs of the project context. IP only
   I implement my CI/CD pipeline using github actions.
   I chose to use github actions because I also use github as version control,
   which makes it easy to do CI/CD here as well.
   The CI/CD takes care of building, testing and deploying the backend.
   And this fully automatically with every push to the git.
   Below I will explain what each piece of the YAML file does.
   The YAML starts with the name of the workflow and when it is executed.
   In this case, it performs this workflow with every push to the master branch.
   | ![image](https://user-images.githubusercontent.com/84378377/171658095-5c62d311-f0b6-4476-8c07-d4766fdaa260.png) | 
   | :--: |
   | _First part of the YAML file_ |  
   
   Next comes the jobs section with the build as the first job.
   In the build, he will build and test the app.
   So he starts with the restore of the dependencies.
   Then he builds and tests the app.
   Once this is successful, it saves the build for later use in publishing the app.
   | ![image](https://user-images.githubusercontent.com/84378377/171658275-f48339a3-1ef7-460c-99f4-4f2e80fbf178.png) | 
   | :--: |
   | _Build part of the YAML file_ |  
   
   Now that he has finished the build job, he will move on to the publish job.
   In the publish job, it starts with the retrieval of the saved build.
   he will then push this build via ftp to the venus server at Fontys.
   | ![image](https://user-images.githubusercontent.com/84378377/171658449-1d4f86e7-8d12-4fdb-8dbb-91791a5f0b16.png) | 
   | :--: |
   | _Publish part of the YAML file_ |  
   
   To ensure that not everyone has the username and password for the ftp server, I store them in the secrets of github.
   This means that only github can access these values and not the users.
   | ![image](https://user-images.githubusercontent.com/84378377/171659024-80112259-e3a6-4324-8722-c9f5cb9a5ce4.png) | 
   | :--: |
   | _Github secrets_ |  
   
   Deployment did not go well at first, which caused the publish to fail.
   Through try and error, I got it to work.
   This is also seen in the action history as the publish succeeded only after several tries.
   | ![image](https://user-images.githubusercontent.com/84378377/171658857-c3fc0a55-fdc6-49fb-8474-218c846acd94.png) | 
   | :--: |
   | _Action history_ |     
      
   I have created a second workflow for the scan of Sonar Cloud.   
   This is a separate workflow from the workflow above.   
   This workflow only takes care of the code scan.   
   | ![image](https://user-images.githubusercontent.com/84378377/172840712-bc2ee289-06bb-4e50-b1cb-a248cb8a6183.png) | 
   | :--: |
   | _Sonar Cloud workflow_ | 
    
## 8 You act in a professional manner during software development and learning. IP and GP
   To get feedback from my teachers about my work I try to get a feedback moment every 2 weeks.
   In the start of the semester this wasn't going very well, I had my first feedback moment after 3 weeks into the semester.
   To compensate for this low amount of feedback moments For a few weeks I planned a moment very week.
   Now I have at least a feedback moment every 2 weeks and if needed every week.
   One of my teachers(Jean Paul) uses feedpulse to keep track of the feedback moments.
   
   | ![image](https://user-images.githubusercontent.com/84378377/172840785-f22ae9ab-c5c9-4d8e-b7e2-b2d5d18a30e5.png) | 
   | :--: |
   | _Feedpulse_ |  
   
   Beside this, I choose the specialisation education which means I need to get an internship at a school.
   To achieve this i had to write an resume and multiple application letters.
