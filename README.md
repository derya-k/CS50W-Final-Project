# CS50W Final Project 
In this project, I developed a web application called "ART+".This application is a platform where articles on different branches of art can be uploaded.The articles uploaded in this application remain live for two weeks. If you want to access these articles later, you should like these articles.I wanted to develop an easy-to-examine, uncomplicated web application for anyone interested in art. With this application, it is aimed to give an idea to people in general thanks to the short and concise articles.

In this web application Django, Javascript and Bootstrap, were used and web application is mobile-responsive.
In the distribution code is a Django project called capstone that contains a single app called blog.

#### What makes this project more complex than the others?
In this project, in addition to the other projects I developed during the course, I focused on the front-end part.I tried to develop a web application that provides a more aesthetic look and a better user experience.I wanted to develop an application that is simple but does not skip any required content.
It is the first application I designed as mobile responsive.

### How to run this web application 
It must first be installed  python and django on your computer
Run "python manage.py runserver" in your terminal to start up the Django web server, and visit the website in your browser.

### Structure of Web Application 

- **Models**:Application have five models. One for users, one for posts,one for categories,one for comments made on posts, one for contact. 
    - Related files:
        -blog/models.py

- **About Us Page**: In this page there is an explanation why this web application built.
    "*ART+ is a platform where you can follow current developments in the art world.We want to bring you both    current and creative content.
    Articles published on ART+ will only stay on the platform for two weeks.
    If you want to access content after two weeks, you must like the content.*"
    - Related files:
        - Html file: blog/templates/blog/aboutus.html
        - Css file: blog/static/blog/css/aboutus.css and bootstrap.min.css
        - Javascript file: blog/static/blog/js/aboutus.js

- **İndex Page**: This is a default page. Users can view the articles and related images posted on this page, with the most recent posts first. Any user can click on any article's title or related image to be taken directly to that article page.If user not logged in, navbar shows log in and register buttons.
    - **Register Page**: User can become a member by entering their username, e-mail address and password.
    - **Log In Page**: If user is register, he/she can log in with username and password.
    - **Log out**: User can log out by clicking the log out button in the navbar
    - After the user is logged in, Profile and Liked pages appear in the navbar.
    - Users can like posts after they sign in.(Javascript were use for that)
    - For every published article; if the article is longer than 20 words, the first 20 words, category, image, author, number of likes and publication date appear on the index page.(Javascript were use for that)
    - Related files:
        - Html file: blog/templates/blog/index.html
        - Css file: blog/static/blog/css/style.css and bootstrap.min.css
        - Javascript file: blog/static/blog/js/main.js

- **Profile Page**: In this page, the user can see all the articles she/he has uploaded,  with the most recent posts first.The user can click the "create new article" button to open the form required to upload a new article, .Title, content, (image is optional) and category sections in this form must be filled in order to compose the article.
    - Related files:
        - Html file: blog/templates/blog/profile.html
        - Css file: blog/static/blog/css/style.css and bootstrap.min.css
        - Javascript file: blog/static/blog/js/main.js

- **Liked Page**: User can always see all the articles she/he liked on this page.
    - Related files:
        - Html file: blog/templates/blog/profile.html
        - Css file: blog/static/blog/css/style.css and bootstrap.min.css
        - Javascript file: blog/static/blog/js/main.js


- **Category**:There is a dropdown on the navbar to see all categories. Clicking on any category will show all the articles in that category.

- **Contact Page**:Users can send a message to the admin from this page.
    - Related files:
        - Html file: blog/templates/blog/contact.html
        - Css file: blog/static/blog/css/style.css and bootstrap.min.css
        

- **Article Page**:This page contains the entire article, the image, the name of the author, the date the article was published.You can also view all comments by clicking the "show comment" button and comment by clicking the "comment" button.
    - Related files:
        - Html file: blog/templates/blog/article.html
        - Css file: blog/static/blog/css/style.css and bootstrap.min.css
        - Javascript file: blog/static/blog/js/article.js

- **Comment**:When users enter the article page, they can comment and see on all comments made. User who made the comment and the date the comment was made are visible in the comment section.






