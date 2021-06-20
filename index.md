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

Here's what my application looked like once I was finished with the design layout:
Login Screen: 
![Screen Shot 2021-06-20 at 11 37 15 AM](https://user-images.githubusercontent.com/37714835/122681860-f84fc900-d1bb-11eb-9b1e-a67e529261e3.png)
Charts Fragment: 
<img width="329" alt="Screen Shot 2021-06-20 at 11 35 48 AM" src="https://user-images.githubusercontent.com/37714835/122681870-06054e80-d1bc-11eb-8c50-e8dbabddaf22.png">
Enter Weight: 
<img width="327" alt="Screen Shot 2021-06-20 at 11 35 59 AM" src="https://user-images.githubusercontent.com/37714835/122681880-0ef62000-d1bc-11eb-9d08-3272faf96125.png">
Weight Log: 
<img width="327" alt="Screen Shot 2021-06-20 at 11 36 09 AM" src="https://user-images.githubusercontent.com/37714835/122681891-1caba580-d1bc-11eb-8d5e-a9755fc6a57b.png">
Settings:
<img width="333" alt="Screen Shot 2021-06-20 at 11 36 18 AM" src="https://user-images.githubusercontent.com/37714835/122681901-246b4a00-d1bc-11eb-9917-1155591bcffa.png">
<br/>

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
