## Joshua M Gierlich

During my educational career at SNHU I have taken numerous courses. Each course brought greater understanding about information technology in a broad sense. As I have gotten closer to the end of my degree the classes have been much more specific in their content, and have included many aspects of courses that I have taken prior. One class in particular was my CS-360 Mobile Architect and Programming course which had us create an Android application. I chose to create a weight tracking application, which incorporated using buil-in databases to track a users progress, and used the databases incorporated in the application to authenticate the user. To make the application meant designing an application, creating the functionality for each buttton/page using java, and incorporating secure coding practices to each script created. We were tasked with improving our applications and listed below are some examples showing how I met each of the critera mentioned.  <br/>

### Code Review 1  <br/>
[Code Review Link](https://www.youtube.com/watch?v=AZMZ0pc8V3w)


### Capstone Artifact #1 - Software Engineering and Design

In my first attempt at creating the application I was mainly focused on getting a usable application, and in doing so had left a lot to be desired especially regarding design. My application initially had three windows, and each had a dedicated function (logging weight, adding weight, and setting a target weight) with limited capacity. The application was strictly a user interface meant to store data and nothing else. The application functioned appropriately but I really disliked the color scheme, and while the layout was direct, I believed that it could have been improved upon. 

Here's what my application Initially looked like:

<img width="321" alt="Screen Shot 2021-06-20 at 11 21 01 AM" src="https://user-images.githubusercontent.com/37714835/122681489-26340e00-d1ba-11eb-9d7a-489f0cce9904.png">
<img width="317" alt="Screen Shot 2021-06-20 at 11 21 43 AM" src="https://user-images.githubusercontent.com/37714835/122681503-2fbd7600-d1ba-11eb-97f8-e73502988c18.png">
<img width="317" alt="Screen Shot 2021-06-20 at 11 22 00 AM" src="https://user-images.githubusercontent.com/37714835/122681508-34822a00-d1ba-11eb-9ad2-544206fce2b3.png">
<img width="322" alt="Screen Shot 2021-06-20 at 11 22 08 AM" src="https://user-images.githubusercontent.com/37714835/122681511-377d1a80-d1ba-11eb-8adb-be155789a0ee.png">

As you can see, a login was the same as creating an account, and in the background there was really no validation except to determine if the same username and password existed in the database. This also presented challenges because if a person logged in accidentally under a different username or password, a new account would be created for them even if they simply just wanted to log into their own account. I needed some additional validation to make my program stronger, more secure and more reliable for the end user. 


Once I had started this project I first set out to change the color scheme and design layout I changed the color scheme from a bright layout, using googles preset color scheme to a darker layout for a sleeker look. I wanted the user to be able to visually track their progress, make predictions, and use statistics to map their progress. To do this I needed to add new fragments and code to support the functionality for each fragment. I also wanted some new features to support to ensure a much easier to use application so I added an SMS feature to log in as well as an email so that the user could choose how they would like to log in. These few changes made it easier for me to authenticate each user and establish metrics later on to help me determine what method people liked to use more for each application. Much of the changes that I did end up making for receiving user input was created to eliminate bad user input. For instance, in my initial application the person could enter a date however they saw fit, whereas with m new application the user had to choose from an actual calendar which then formatted the date for the person. All in all I believe that I created a much more enjoyable end user experience, while aslo adding plenty of new functionaloity for additional development later on as well.   

Here's what my application looked like once I was finished with the design layout:<br/>

Login Screen: 


![Screen Shot 2021-06-20 at 11 37 15 AM](https://user-images.githubusercontent.com/37714835/122681860-f84fc900-d1bb-11eb-9b1e-a67e529261e3.png)
<br/>

Charts Fragment: 


<img width="329" alt="Screen Shot 2021-06-20 at 11 35 48 AM" src="https://user-images.githubusercontent.com/37714835/122681870-06054e80-d1bc-11eb-8c50-e8dbabddaf22.png">
<br/>

Enter Weight: 


<img width="327" alt="Screen Shot 2021-06-20 at 11 35 59 AM" src="https://user-images.githubusercontent.com/37714835/122681880-0ef62000-d1bc-11eb-9d08-3272faf96125.png">
<br/>

Weight Log: 


<img width="327" alt="Screen Shot 2021-06-20 at 11 36 09 AM" src="https://user-images.githubusercontent.com/37714835/122681891-1caba580-d1bc-11eb-8d5e-a9755fc6a57b.png">
<br/>

Settings:


<img width="333" alt="Screen Shot 2021-06-20 at 11 36 18 AM" src="https://user-images.githubusercontent.com/37714835/122681901-246b4a00-d1bc-11eb-9917-1155591bcffa.png">
<br/>

I really struggled a lot with implementing this new design, espescially as I continued to build new functions and features into the application, because each new component required new code to create. Oftentimes I would get lost on what I was working on and had to stop and review what I had created. In many cases I literally had to draw out the connections of each element to understand what wasn't yet connected and as you can see in some parts of my programming, I had put in exceptions to understand what kind of errors I was running into. In some cases I found the exceptions useful, and instead of getting rid of them, I actually incorporated them into the logic, so that the user understands what he/she didn't do correctly, which makes the application even easier to use. Some aspects of my design were purely aeshetic 
while others were designed to minimize errors, and some are experiments or meant for further development during later iterations (like the settings layout for instance). This project really helped me learn how I problem solve with large integrated projects. I utilized a lot of visualization tools initially and spent a lot of time in the planning and static coding phases so that I had a clear path before I continued. I did enjoy this agile method of development, and I utilized a lot of agile methodology to iterate, and make new versions of each part of my application. 

### Capstone Artifact #2 - Data Structures and Algorithms: <br/>

One realization that I had once I created my initial application was that by using a relational database on each users local device, I would quickly lose visibility on my application once it was downloaded on an end users' device, meaning I would lose potential reporting aspects that would provide crucial insights into how I might want to improve upon the application in later iterations. Initially, I had incorporated three databases (users, daily_weight, and target_weight). I found this setup to be comfortable and I really liked how easily understandable it was. My goal during the next iteration was to find a better method to track multiple devices but still provide the same functionality to the end users using my application. I needed a way to communicate securely to a remote database which could store the information I needed, and the most direct solution that I could come up with was using an API. After some research I found an application called "Firebase" which hosts an API that would be able to provide the necessary storage and also provided ready made reporting tools meant to track just the type of information that I was trying to track. In addition the application also supported the ability to report application failures or problems which is something that I found very appealing. 
<br/> 

Another benefit of utilizing a remote database is security. Android comes standard with a set of libraries that are able to check/validate for specific types of responses which my initial application lacked. I was able to account for whether or not a persons input was a valid email address, or phone number, and if the users input didn't match the specified criteria would give the user an error. In addition, instead of simply creating a new user every time a match wasn't found the user is prompted to either put in known credentials to get access to their account, or create a new account with new credentials. This made my program much more secure by not storing all users' data on a local database, and instead ensured that only the authorized users information was accessed every time. 

Ultimately I ended up with one table as much of the metadata that I was interested was populated in other tables created by Firebase which made it much simpler for me as I only needed to create the functionality within the application, rather than having to also program the databases which would house the metadata that I was ultimately interested in. 

What I found really challenging at first was figuring out how many databases to create. At one point I had mapped out five databases, and found myself configuring the program to linearly search through each one on the users ID. It wasn't until much later after some testing that I found out that Firebase supported the reporting I was looking for all on its own. From there the next challenge was getting the auth credentials configured correctly to work every time, and then to populate the correct fields. Once I was able to figure that out, the next challenge was simply creating modules to call so that I could easily make calculations which I defined in a "Data Definitions" Java file. I relied heavily on these definitions within the Chart Java files, and "Statistics" Java files whereas before this I was going to make specific SQL commands to calculate the necessary fields, and then reference those fields as necessary. I tinkered with this approach for a while but I didn't like the idea of having to consult different scripts outside of my application to see if there was issue. <br/>

Below are examples of scripts I used utilizing the API, the API interface, and how I implemented some of the more complicated features of my application:
[API Client](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/APIClient.java)<br/>
[AccountFragment](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/AccountFragment.java)<br/>
[Base_Activity](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/Base_Activity.java)<br/>
[ChartFullScreen](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/ChartFullScreen.java)<br/>
[ChartStatistics](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/ChartStatistics.java)<br/>
[ChartUtils](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/ChartUtils.java)<br/>
[ChartsFragment](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/ChartsFragment.java)<br/>
[DataDefinitions](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/DataDefinitions.Java)<br/>
[EmailLoginFragment](https://github.com/tweedleduh/tweedleduh.github.io/blob/main/EmailLoginFragment.java)<br/>

These files in particular required a large amount of integration and forethought. While some of the programs I initially had bits and pieces of, because of the added chart, statistics, login options, and API integration resulted in me having to write most of the code from scratch. This should show that not only do I recognize possible security threats, but I can also securely connect to and utilize third party software to cater to the needs of not only the end users, but also to potential business partners. I built each script modularly, so that it can be utilized as often as needed. The included code shows how I implemented the data interface, and how I could easily build out additional features to cater to the future needs of the application and potential business partners, should there be any in the future <br/>



You can use the [editor on GitHub](https://github.com/tweedleduh/tweedleduh.github.io/edit/main/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/tweedleduh/tweedleduh.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
