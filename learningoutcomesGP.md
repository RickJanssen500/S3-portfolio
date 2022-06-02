

## Learning outcomes

   ## 1 You design and build user-friendly, full-stack web applications. IP and GP
   - User-friendly  
   
      In LO6 I show a few design choices about making the views user-friendly.
      For the frontend I installed the css-framework bootstrap, and made sure every element uses the correct styling.
      By using bootstrap the styling looks good and is user-friendly because it wil automaticly scale to the device's screen.
      | ![image](https://user-images.githubusercontent.com/84378377/171585887-49c49364-6770-4d31-834e-525beb640569.png) | 
      | :--: |
      | _Our bootstrap button bar_ |   
      
      To let the user know something went wrong or cann't be done, I made multiple (error) message's.
      So the user knows what happend. below I will show you the 2 tipe's of messages I created.
      | ![image](https://user-images.githubusercontent.com/84378377/171587561-a9c6073f-87d9-49fe-8a80-ef8d251de7b7.png) | 
      | :--: |
      | _no data error_ |  
      
      This error Shows there is no data for the selected date and/or the selected floor. So the user will know it needs to change there settings to see data.   
      
      | ![image](https://user-images.githubusercontent.com/84378377/171587656-f16ce233-ca3f-4b79-b88d-9b8a8c5798f7.png) | 
      | :--: |
      | _trying out the future message_ |    
      
      This message shows that the time the user selected is in the future, 
      the system automaticly changed the dat/Time to the now posistion and shows the user the messsage as shown up here.   
        
      ### - Full-stack  
   
      For the appilication I made the heatmap using Highchart. I set everything up so the data would be displayed in the right color and in the right position in the map.
      
      For the error message above I wrote a function that checks if the date is in the future. 
      If this is the case it wil set the time/date to now and show the user the message.
      If the time is not in the future this function make sure the message is not shown to the user anymore   
      | ![image](https://user-images.githubusercontent.com/84378377/171589348-f6ca2344-fe25-4262-aca1-5c8a1e046972.png) | 
      | :--: |
      | _Time in future function_ |  
      
      
      
   ## 3 You choose and implement the most suitable agile software development method for your software project. GP only
   
   We work in an agile process in our group project. Every Day we start with the daily stand-up, mostly around 09:30 because the group is complete by then.
   Here we will discuss what everyone has been/will be doing for the day and where we currently stand in the project and what still needs to be done this sprint.
   We will take a look at our notion board and look who is assigned to which task. If somebody isn't assigned to any task, we deside to which task he will we assigned to.
   At the end of the day we have a daily stand-down. Here we will discuss how everything went this day and the progress everyone booked.
   Sometimes we also have meetings before or after lunch break to make sure everyone can keep working and won't get stuck add a problem.
| <img src="https://user-images.githubusercontent.com/58734636/164235377-e98aad38-8905-4ecb-aa04-9e9170b56239.png" width="700" height="600" />| 
| :--: |
| _Screenshot of our notion board_ |

We end every sprint with a sprint review and a sprint retrospective. The sprint review is with the product owner.
We will deliver our work from the sprint and get feedback from the product owner.
then we discuss what we are aiming to do next sprint and see if it is in line with the client's expectations.
After the sprint review we will do the sprint retrospective.
In which we will look at what went well, what can be improved and what went bad. We do this by asking ourselves a lot of questions.
We then adapt our working methods to the findings of the retrospective.
| <img src="https://scrumorg-website-prod.s3.amazonaws.com/drupal/inline-images/2021-01/scrumorg-scrum-framework-3000.png" width="800" height="500" />| 
| :--: |
| _The scrum workflow we apply in our project_ |
   

   ## 5 You recognize and take into account cultural differences between project stakeholders and ethical aspects in software development. GP only
   
Software engineering consists of subjects outside of coding and documenting.
One such subject is the cultural and ethical values that play a role in a professional environment, 
and the importance of these values in creating and maintaining a comfortable working environment.

#### Ethics

**What is ethics in software engineering?**  
Ethics, as described by Oxford Languages, is a set of moral principles that govern the behaviour of a person or the conduction of an activity. 
Ethics are used to measure the righteousness of an action, acting as criteria for judging whether something is right or not. In the scope of software engineering, 
ethics dictate the values a software engineer should adhere to in a professional environment. This includes ethics related to cultural differences, software,
source code and communication.

**Why is ethics important in software engineering?**   
Ethics in software engineering can be viewed from multiple perspectives. One of these perspectives is that of the production environment.
Another one would be that of the product (and it’s users).
The ethical values adhered to during the production of a product define the workability and comfortability of the environment.
A lack of proper ethical values or a lack of enforcing them will eventually create a working environment where discrimination, bullying,
favouritism among other things are allowed. For this reason, it is important for proper, unanimously agreed upon ethical values to be present.
The ethical values the product adheres to at it’s core define how an application could impact it’s users.
An application built with strong ethical values at it’s core should result in a product that will affect users in a positive manner,
whereas one that lacks this core may result in the opposite reaction. 
For this reason, it is important to consider how users could be negatively impacted by something, and what can be done to minimize this reaction.

**What do you have to do as a software engineer to address ethical aspects in your work?**  
Within the software engineering space, a number of widely used ethical guidelines can be found on the internet. One such guideline is the [ACM Software Engineering Code of Ethics](https://ethics.acm.org/code-of-ethics/software-engineering-code/), which states that software engineers should strife to analyze, design, develop, test and maintain software in a truthful, upfront and professional manner for the better of public health, safety and welfare of humanity, according to the following eight principles: 
1. PUBLIC – Software engineers shall act consistently with the public interest.
2. CLIENT AND EMPLOYER – Software engineers shall act in a manner that is in the best interests of their client and employer consistent with the public interest.
3. PRODUCT – Software engineers shall ensure that their products and related modifications meet the highest professional standards possible.
4. JUDGMENT – Software engineers shall maintain integrity and independence in their professional judgment.
5. MANAGEMENT – Software engineering managers and leaders shall subscribe to and promote an ethical approach to the management of software development and      maintenance.
6. PROFESSION – Software engineers shall advance the integrity and reputation of the profession consistent with the public interest.
7. COLLEAGUES – Software engineers shall be fair to and supportive of their colleagues.
8. SELF – Software engineers shall participate in lifelong learning regarding the practice of their profession and shall promote an ethical approach to the practice of the profession.

**How do you know that your ethical considerations match with those of other software engineers?**  
In order to verify all software engineers ethical values match up, it is important for all parties involved to converse about the topic. 
Allowing everyone to share their ethical values and boundaries with one another makes it possible 
to create a working environment in which all parties involved can work comfortably.

**Which ethical aspects play a role in your project?**   
One of the ethical aspects in our group project that we faced was the licensing of third party libraries(Highcharts).
As our project lives in a gray area between commercial and non-profit
(the organization is a business, while the application is strictly for internal use without any direct link to generating profit),
we considered whether purchasing a license for these libraries would be necessary.

**Do you foresee ethical conflicts caused by your software? What kind of?**   
I do not expect any ethical conflicts in our project. Beacause our project displays temparature and humidity levels.
By just giving a temperature I don't think we will cause any ethical conflicts.

**Can you do something to avoid or minimize these conflicts?**  
Communicating regularly with one another is key in preventing (or solving) conflicts in a professional setting.
Expressing one’s concerns and problems spreads awareness to all parties involved and allows them to seek out a solution together.
It also minimizes the amount of misunderstandings that could potentially happen.

#### Culture

  **What is culture?**   
  *"Culture encompasses religion, food, what we wear, how we wear it, our language, marriage, music, what we believe is right or wrong, how we sit at the table,
  how we greet visitors, how we behave with loved ones and a million other things,"* - Cristina De Rossi, an anthropologist at Barnet and Southgate College in London.
  
  **Which are well-known dimensions on cultural differences?**  
  The 6 well-known culture dimensions of Hofstede are:
  
  - Power distance
  Power distance is the degree a society accepts or rejects the unequal distribution of power in organisations and society. In high power distance cultures such as Japan,
  we expect to find great respect for age, status and titles. This could create problems for an American visitor used to the informality of a more moderate power distance
  culture, and accustomed to using first names and casual dress in the office.

- Uncertainty Avoidance
Uncertainty avoidance is the degree a society tolerates or is uncomfortable with risk, change, and situational uncertainty. 
In high uncertainty avoidance cultures, such as France or Japan, one would expect to find a preference for structure, order and predictability.

- Individualism-Collectivism
Individualism-collectivism is the degree to which a society emphasises an individual’s accomplishments and self-interest, 
versus the accomplishments and interests of groups. In Hofstede’s data, the United States had the highest individualism score of any country.

- Masculinity-Femininity
Masculinity-femininity is the degree a society values assertiveness and materialism versus feelings, relationships, and quality of life. 
You might think of it as a tendency to emphasise stereotypical masculine or feminine traits and attitudes towards gender roles. 
Visitors to Japan, with the highest masculinity score in Hofstede’s research, will probably notice how restricted career opportunities can be for women.

- Time Orientation
This is the degree to which a society emphasises short-term or long-term goals. Americans are notorious for being impatient and wanting quick, even instant gratification.
Accordingly, American companies are expected to achieve short-term results. Many Asian cultures are the opposite, valuing persistence, being patient,
and are willing to work for long-term success. 

- Indulgence-Restraint
The Indulgence dimension is a relatively new dimension to the model. This dimension is defined as the extent to which people try to control their desires and impulses,
based on the way they were raised. Relatively weak control is called Indulgence and relatively strong control is called Restraint. Cultures can, therefore,
be described as Indulgent or Restrained. Indulgence stands for a society that allows relatively free gratification of basic and natural human drives related
to enjoying life and having fun. Restraint stands for a society that suppresses gratification of needs and regulates it by means of strict social norms.

*Source : [Hofstede's cultural dimensions](https://www.business-to-you.com/hofstedes-cultural-dimensions/)*
  
  **Can you give examples for cultural differences that you have experienced in your study or life? How do you explain these differences?**  
  I have been on a holiday in India. Where we(Dutch) just shake hands to greet each other, the Indians bow to each other and only shake hands with their best friend.
  This comes from their religion because they also greet God in this way and they have adopted it in their daily lives instead of shaking hands as we do.
  
  **What is your culture?**  
   nog invullen
   
  **What did you do to improve the group communications with respect to cultural differences?**  
   We all share the same culture, so we didn't need to adapt to each other. We sometimes switch language from Dutch to english because it's better for some of us.

   ## 6 You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using multiple types of test techniques. GP only  
   In our group project we try to get as much feedback from the client, so we stay on track with the cumstomers expectations. 
   we try to plan a meeting every week to achieve this. Because we have a weekly meeting, we quickly notice if we deviate from the customer's expectations.   
   
   For the group project, I made a design for the dashboard. In the first design, I also included the maximum and minimum temperature and humidity.
   I presented this to the group members and the client. 
   with the feedback I received on this, 
   So the client didn't want a max/min temperature and humidity on the sreen. He want to focus on a temperatur/humidity on specific locations.
   I modified the design and then asked for feedback on this again from both group members and the client. 
   Until we had come to the final design. with which the client is happy. 


   | <img src="https://user-images.githubusercontent.com/84378377/170023857-af6d8429-8a90-4b6c-9156-2f0b51c8b015.png" width="640" height="360" />| 
   | :--: |
   | _First dashboard design_ |
   
   | <img src="https://user-images.githubusercontent.com/84378377/170024926-e87c7718-98fc-4826-a4ca-99ea7443b6b9.png" width="640" height="360" />| 
   | :--: |
   | _Final dashboard design_ |
   
   For the temperature legend, I came up with the 2 different ways.   
   The first way is that the min and max values move with the min and max of the data on the current map.
   In the second way the legend min and max have a fixed value so the contrast gets less but the contrast stays the same at different times.
   After presenting this choice to the customer, the customer chose the second way. 
   
   | <img src="https://user-images.githubusercontent.com/84378377/170029262-3282744a-0d85-4711-abb0-c3f17206d8ea.png" width="262" height="67" />| 
   | :--: |
   | _Temperature legend_ |

   ## 7 You analyze and describe simple business processes that are related to your project. GP only
   
   In our group project we couldn't find a business project we can analyze. So we discussed this problem with our teacher (Marc) and came to the conclusion that we
   should analyze any relevant business project. So we as a group analyzed the business process of order picking. Webshops have huge warehouses filled with products that 
   can be ordered and picked. Advanced algorithm's create picking lists for employees to pick. We visualized this process for multiple reasons. First of all it's Rens his
   job. And it was easy for Rens to guide us in analyzing this process. Second of all, I created an order-picking system for my individual project. These two reasons let us
   to the decision for our business process to analyze. Which is shown below.
   | <img src="https://user-images.githubusercontent.com/84378377/169816086-8f6a4b9c-7ae7-43ae-bdb1-71b24586a1d8.png" width="1500" height="300" />| 
   | :--: |
   | _The Business process we analysed for our project_ |
   
   We made the process in Engage Process Modeler, because we used this tool before in S1.
   We choose to keep it simple and clear. As a group we set down and discussed the process until
   we all had a clear view of the process and everyone shared the same opinion. 
     
   ## 8 You act in a professional manner during software development and learning. IP and GP
   
   As seen in LO3, we use the scrum methodology as we hold daily stand-ups, stand-downs, sprint reviews, sprint retrospective etc.

   I always try to communicate professionally and in a timely manner with my group members, as well as with the product owners.
   If my train is delayed I will let my groupmembers know I will be a bit later. 
   I'll do this via Whatsapp because this is a fast way to communicate with my group members in case something like this happens.

   If we know a groupmember can't make it to school, we wil do the meeting in Discord so everyone is able to participate in the standup/standdown.
   So they will still be able to track our progress as well as share their own.

   In the earlier meetings I did not talk a lot during meetings with the stakeholder. 
   While we were trying to switch between who leads the meeting, Rens would be the meeting leader most of the time.
   During one week of the semester Rens was on holiday during a meeting with our stakeholder, This forced me to take a more leading role in the meeting.
   Since this meeting I have been more active in the meetings, with showing our work and dicussing with the stakeholder.

