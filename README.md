# Milestone-Project-4
<p align="center"><strong>Milestone Project </strong>

<p align="center"><strong>Full Stack Framework With Django</strong> 

<p align="center"><strong>Code Institute</strong>

<p align="center"><strong>DevMuscles</strong> 

An online commerce site where users can buy items relating to fitness(fitnesswear, equipment, plans etc).
The project has a couple of pages:

1:A homepage that allows users to search for items relating to fitness, and view the products in detail.

2:A login page where users can either login or register for an account.

3:Profile page where the user can update their delivery details and see the orders they have made on the site.

4:Page where the admin can edit/delete products that were created on the site.

5:Page where the admin of the site can add or edit categories.

[Link to website](https://milestone-project-four-muscles.herokuapp.com/) here to see the website.

![Website](images/DevMuscles.png)

## Table of Contents
> - [UX](#ux)
> - [User Stories](#user-stories)
> - [Strategy](#strategy)
> - [Scope](#scope)
> - [Technologies Used](#technologies-used)
> - [Libraries](#libraries)
> - [Version Control](#version-control)
> - [Other](#other)
> - [Testing](#testing)
> - [Deployment](#deployment)
> - [Credits](#credits)
> - [Acknowledgments](#acknowledgments)

## UX:

## User Stories:
As a User/Admin:

"I want to see all the products on the site"

![Products](images/all_products.png)

As a User:

"I want to be able to signin into the site using an account i created"

![Signin](images/user_signin.png)

![Signin Result](images/user_signin_result.png)

"I want to be able to signout of the site"

![Signout](images/user_signout.png)

![Signout Result](images/user_signout_result.png)

"I want to be able to add a product i would like to buy on the site to a shopping bag"

![Add Product to Bag](images/user_add_to_bag.png)

![Add Result](images/user_add_to_bag_result.png)

"I want to be able to search for a product on the site"

![Search Product](images/user_product_search.png)

![Search Result](images/user_product_search_result.png)

"I want to be able to go to my profile and update my delivery details and see any orders i have made"

![Profile](images/user_profile.png)

"I want to see a product in more detail"

![Product Detail](images/user_product_detail.png)

"I want to be able to edit my shopping bag before it goes to checkout"

![Edit Shopping Bag](images/user_edit_bag.png)

"I want to look for products in certain areas instead of having to look at all of them"

![Product Categories](images/user_products_navigation.png)

As an Admin:

"I want to be able to delete products from the site"

![Delete Product](images/admin_delete_products.png)

![Delete Product Message](images/admin_delete_product_message.png)

"I want to be able to edit products on the site"

![Edit Products](images/admin_edit_products.png)

## Strategy:
I wanted to create a user friendly website that would have Create,Update,Read and Delete (CRUD) functionality as well as site that would accept payments.

## Scope:
I created a database for the products and categories,see below schemas

![Category Schema](images/categories_db.png)

![Product Schema](images/products_db.png)

## Technologies Used:
[HTML](https://html.com/)
Used to create the structure of the web site.

[CSS](https://www.w3schools.com/css/css_intro.asp)
Used to style the website.

[Python](https://www.python.org/)
Used to create the CRUD functionality.

[Bootstrap](https://getbootstrap.com/)
Used to design the site for mobile users and for other features.

[Stripe](https://stripe.com/)
Used to handle credit card payments on the site

[Heroku](https://id.heroku.com/login)
Used to host the site.

## Libraries:
[Django](https://www.djangoproject.com/)
Used for the main development of the site.

[WhiteNoise](http://whitenoise.evans.io/en/stable/#)
Used for the collecting and storing of staticfiles.

## Version Control:
[Github](https://github.com/) - Used to store the code and use of Github Pages to deploy the website. 

[Gitpod](https://gitpod.io/) - Used as the primary version control IDE for development to further push and commit code to Gihub.

## Other:
[Code Institute Course Content](https://courses.codeinstitute.net/) - Primary source of learning code.

[W3Schools](https://www.w3schools.com/) - used as a general resource for CSS and coding tips.

[StackOverFlow](https://stackoverflow.com/) - used as a general resource for layout tips or questions.

## Testing:
<p align="center"><strong>Manual Testing of the site</strong></p>
The project was tested on a smartphone, a Desktop computer and a Samsung Tablet.

It was also tested on 3 web browsers: Google Chrome, Mozilla Firefox and Microsoft Edge.

<p align="center"><strong> HTML Validation</strong></p>

HTML - [W3C](https://validator.w3.org/) - Markup Validation.

![Homepage](images/html_validation.png)

![Add Products](images/html_validation_add_product.png)

![Shopping Bag](images/html_validation_bag.png)

![Checkout](images/html_validation_checkout.png)

![Edit Product](images/html_validation_edit_product.png)

![Equipment](images/html_validation_equipment.png)

![Fitnessswear](images/html_validation_fitnesswear.png)

![Login](images/html_validation_login.png)

![Nutrition](images/html_validation_nutrition.png)

![Products](images/html_validation_products.png)

![Profile](images/html_validation_profile.png)

![Signout](images/html_validation_signout.png)

![Workout](images/html_validation_workout.png)

<p align="center"><strong> CSS Validation</strong></p>

CSS - [W3C](https://jigsaw.w3.org/css-validator/) - CSS Validation.

[Validation Result](images/css_validation.png)

## Deployment:
I did the following to deploy my site:

Removed all my hard-coded environment variables. 

These were placed in the Heroku Config Vars for production.

Ensured the applications requirements.txt is up-to-date with all the latest packages installed for my app being noted on this file.

The command to update requirements  is pip3 freeze > requirements.txt

Ran the command python manage.py loaddata for the categories and products files in the fixtures folder to add them to the Django database 

Ran the command python manage.py collectstatic in order to collect all the images, JavaScript and CSS files in the project and place them into the static files to be used for Heroku

Set up the Procfile - A Procfile is required by Heroku in order to tell the service worker what command to run for my application to start.

Set Django's debugging to False.

Pushed all my latest production ready code to GitHub ready for deployment via Heroku's GitHub function where you can deploy from GitHub the production ready app.

Upon successful deployment Heroku will give you the URL that is hosted your app

If you want to create a copy of this site on GitHub,do the following:

To access the code, it can be run locally by either selecting "clone" which provides an URL one can use on their local machine or "download" which is where one can download the zip file on to their machine.

Install the projects requirements.txt using pip3 install -r requirements.txt

You will need to update a few environment variables before you can run the app.

os.environ.setdefault("DATABASE_URL", "")

os.environ.setdefault("EMAIL_HOST_PASS", "")

os.environ.setdefault("EMAIL_HOST_USER", "")

os.environ.setdefault("SECRET_KEY", "")

os.environ.setdefault("STRIPE_PUBLIC_KEY", "")

os.environ.setdefault("STRIPE_SECRET_KEY", "")

Once the above steps are complete you can try run the application using python3 main.py

## Credits:

## Content:
All text content in this website was written by me.

## Media:
The photos used in this site were obtained from:

Homepage background gotten<a href="https://www.google.com/search?hl=en-IE&tbs=simg:CAQSiQIJPpcIGl5sbUYa_1QELELCMpwgaOgo4CAQSFM0hvTL-PK84iw--HokslR36IeAeGhrv4gxneoTp6JfsCfEo0i-klwsaeYO-5uiihCAFMAQMCxCOrv4IGgoKCAgBEgRrIAfMDAsQne3BCRqdAQojCg9mcmVlIHdlaWdodCBiYXLapYj2AwwKCi9tLzBoOG00YmYKGgoHYmFyYmVsbNqliPYDCwoJL20vMDNfMTYzChkKB3dlaWdodHPapYj2AwoKCC9tLzBoenN2Ch8KC2FjdGl2ZSB0YW5r2qWI9gMMCgovbS8waGdudGd3Ch4KDHBvd2VybGlmdGluZ9qliPYDCgoIL20vMGg1dDQM&q=person+lifting+weights&tbm=isch&sa=X&ved=2ahUKEwj_n_yX86f0AhWUoFwKHUt7BvQQwg4oAHoECAEQMg&biw=1366&bih=587&dpr=1"> here</a>

Xenios USA Fitness Dumbbells gotten<a href="https://www.xeniosusa.com/en/pair-of-fitness-dumbbell.html"> here</a>

Water Bottle gotten<a href="https://eu.gymshark.com/products/gymshark-fruit-infuser-black"> here</a>

Skipping Rope gotten<a href="https://eu.gymshark.com/products/gymshark-skipping-rope-black"> here</a>

Arrival 5 Shorts gotten<a href="https://eu.gymshark.com/products/gymshark-arrival-5-shorts-black-aw21">here</a>

Fit Seamless Shorts gotten<a href="https://eu.gymshark.com/products/gymshark-fit-shorts-black-white"> here</a>

Sports Bra gotten<a href="https://www.decathlon.ie/bras/309915-72862-women-s-cotton-sports-bra-black.html"> here</a>

30 Day Strength Traning gotten<a href="https://www.nbcnews.com/better/lifestyle/30-day-strength-training-routine-no-equipment-required-ncna988936"> here</a>

Warrior Workout gotten<a href="https://ukoutdoorfitness.com/bootcamp/total-warrior-workout-plan"> here</a>

Cardio HIIT gotten<a href="https://www.shape.com/fitness/workouts/cardio-hiit-heart-rate-challenge"> here</a>

30 Day Meal Plan gotten<a href="https://soreyfitness.com/fitness/masters-chisel-calendar-meal-plan/"> here</a>

Vegan bodybuilding gotten<a href="https://www.vivolife.co.uk/blogs/news/a-nutritionist-s-guide-to-a-vegan-bodybuilding-diet"> here</a>

Lean Muscle diet plan gotten<a href="https://healthyrecipesforweghtloss.blogspot.com/2019/08/best-7-day-diet-plan-for-weight-loss.html"> here</a>
  
  
## Acknowledgments:
I received inspiration from an Bootstrap mini project that was taught to us as part of our course.