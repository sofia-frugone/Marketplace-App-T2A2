# README
---
##Makeup Zoo (the problem & the solution: R7/R8)
###As of June 30th 2021, there 2,402,254 actively trading businesses in the Australian economy. 98.4% of Australian businesses are small businesses. The vast majority (93%) of these businesses have a turnover of less than $2 million (afsbeo.gov.au). In Australia, the beauty market had an estimated revenue of $7,756 million in 2021. Most of this revenue goes towards household name brands such as Mecca and Sephora, making it harder for small businesses to compete and turn a profit. Many Australians like to support small businesses however there is no one stop destination for people to browse products from these brands. Makeup Zoo solves that problem and introduces a platform for small business owners to post their listings and get their name out to potential buyers. 
---
##Link to the deployed application
###[Makeup Zoo](https://makeupzoo.herokuapp.com/)
---
##Link to the github repo
###[Github](https://github.com/sofia-frugone/Marketplace-App-T2A2)
---
##Description (R11)
**Purpose:**
Makeup Zoo is a marketplace app which allows its user to buy and sell makeup from small businesses across Australia. 

**Functionality/features:**
View listings: Any user can view listings made on the site, they can see the listing name, description, price and category. To purchase a product the user must have an account with Makeup Zoo.

**Create new listing:**
Users with an account can create new listings. Users can upload an image of their product and set a price when creating the listing. 

**Sign up/in:**
The site has basic sign in and sign up functionality, passwords must be at least 6 characters long. 

**View sold orders:**
Sellers can view what items have been purchased on the sold items page. Sold items are displayed in a table with the initial listing info and buyer username displayed.

**View purchase history:**
Buyers can view their purchase history in a table, similar to the sold orders page, items are displayed in a table with the seller username. 
---
##Sitemap
![Structure Organization Chart Infographic Graph](https://user-images.githubusercontent.com/88522139/178142577-50f021d7-2985-43ec-98e0-297b1028bb56.png)
---
##Screenshots
![homepage](https://user-images.githubusercontent.com/88522139/178142602-06a74c91-2623-4399-9ed3-aaca5c9cb9d7.png)
![listings](https://user-images.githubusercontent.com/88522139/178142608-a248e5c6-f114-4691-a390-475c25d62509.png)
![purchase-history](https://user-images.githubusercontent.com/88522139/178142611-401b0712-3db3-41f6-aa36-8efe78913d93.png)
![sold-items](https://user-images.githubusercontent.com/88522139/178142618-87b8f1ea-eb9d-4d46-9f21-ec4f25462921.png)
![buy-product](https://user-images.githubusercontent.com/88522139/178142624-d770db0a-ea1b-4d51-a3df-9507b29d6a17.png)
![sign-in](https://user-images.githubusercontent.com/88522139/178142634-aac624cc-1f6f-47a0-8f7a-58b4e7541e60.png)
![sign-up](https://user-images.githubusercontent.com/88522139/178142639-c9651926-91ee-4e2f-8b52-4888c267f84d.png)
---
##Target Audience
The target audience for my application is Australians interested in makeup. Particularly makeup collectors who want to support small Australian businesses. My justification for “anyone interested in makeup” is that there is no particular gender or age group that enjoys makeup, it is enjoyed by all different demographics.  

##Tech Stack
Ruby
Html
Css
Tailwind CSS: main framework used for styling
Heroku: deployment platform
Moqu: wireframes
Trello: development tracking
---
##User Stories (R12)

**Listing form:** As a user, I would like to create listings to sell my products.

*Requirements:*
- Signed in user can create listings using the landing page button
- User can add listing name, price and description
- User can add listing category
- User can create listing


**Landing page:** As a user, I would like to view the landing page when I sign in to get a brief overview of the app.

*Requirements:*
- Any user can view the landing page
- Signed in user can sign out 
- Any user can access listings 

**Listings page:**
As a user, I would like to view the listings so I can make a purchase.

*Requirements:*
-Any user can view listings
-Signed in users can purchase a listing
-Users cannot purchase their own listings 
-Signed in users can create a new listing


**Sign in:** As a user, I would like to sign in so I can access listings and the site.

*Requirements:*
- User can sign in using their email and password


**Sign up:** As a user, I would like to sign up for Makeup Zoo so I can access the site and create listings. 

*Requirements:*
- Full Name
- Email
- Password


**Purchase history:** As a buyer, I would like to view my purchase history so that I can get an overview of what I've bought. 

*Requirements:*
-Signed in user can view their purchase history
-Listing title
-Listing description
-Listing price
-Seller username
-Listing category

**Sold orders:**
As a seller, I would like to have a sold orders page so that I can see what products have been purchased. 

*Requirements:*
-Signed in user can view their purchase history
-Listing title
-Listing description
-Listing price
-Buyer username
-Listing category
---
##Wireframes (R13)
![buy-wf](https://user-images.githubusercontent.com/88522139/178142769-5498f3d4-1111-476c-b18a-aed595a47376.png)
![home-wf](https://user-images.githubusercontent.com/88522139/178142771-01fdd173-5192-4a9b-ab74-d5e727be6296.png)
![listings-wf](https://user-images.githubusercontent.com/88522139/178142773-c5e61484-b61c-4f03-9603-176db9aa795b.png)
![mobile-wf](https://user-images.githubusercontent.com/88522139/178142774-abcfd7fe-e6c9-4b27-9119-a4c98ca8361a.png)
![sign-in-up-wf](https://user-images.githubusercontent.com/88522139/178142775-4242073a-5bce-4de4-ab19-b33ad6e9baa8.png)
---
##ERD (R14)
![marketplace-erd](https://user-images.githubusercontent.com/88522139/178142793-10b3dc7b-c3f7-438e-b6bd-31eaca0df93b.png)
---
##Explain the different high-level components (abstractions) in your app (R15)

**Navbar & footer:** The navbar and footer were the most used components in the app. They display on every page. The navbar allows users to navigate easily through the site and the footer was simply a styling decision as all the links are dummy links. 

**Tables:** Tables were used to display listing information on three pages: ‘listings’, ‘purchase history’ and ‘sold items’. It was the simplest way of displaying all the required information. If I were to re-do the assignment I would take more time to look into tailwind utility classes so there is less-repeat inline styling. 

**Forms:** Similar to tables the same form styling was used for sign up, sign and new listing. The sign in and sign up forms are almost identical with minor changes. 
---
##Detail any third party services that your app will use (R16)

Devise: Devise is an authentication solution for Rails based on Warden. It’s a complete MVC solution based on rails that is composed of 10 modules. Devise has been implemented into my app for user registration forms. 
--
##Describe your projects models in terms of the relationships (active record associations) they have with each other (R17)

Users:
The users model was created first so the orders model and listing model could reference the user id for buyers and sellers. has _many specifies a one-to-many association, to demonstrate: a user can have many listings, sold orders and bought orders. 

Categories: 
Categories were created second so the listing model can reference the category_id. 

Listings: 
Listings were created after categories. Listings reference the user_id and category_id. Belongs_to Specifies a one-to-one association with another class. In this case a listing belongs to a user and a category. 

Orders:
Orders were created last and similar to listings specify a one-to-one association with another class. An order belongs to a listing, a buyer and a seller. A foreign key was created for buyers and sellers from the user class. 
---
##Discuss the database relations to be implemented in your application (R18)

There were four tables created for this project: users, listings, categories and orders. 

Users: Users have an optional to many relationship with listings, a user has the ability to create no listings or many listings. Similarly, users have the same relationship with orders. 

Listings: Listings have a one-to-one relationship with users, a user must create a listing and can only belong to that user. Listings have an optional-to-one relationship with orders and categories. The listings table references the user id and category id foreign keys. 

Categories: Categories have an optional-to-many relationship with listings, a category can belong to none or many listings. 

Orders: Orders have a one-to-one relationship with users, an order can belong to only one user and similarly listings. The order table references the listing id, buyer id and seller id foreign key. 
---
##Provide your database schema design (R19)
![marketplace-schema](https://user-images.githubusercontent.com/88522139/178142871-bc480b0b-15fa-4e0d-9a9c-cd7abf2b6c15.png)
---
##Describe the way tasks are allocated and tracked in your project (R20)

Trello was the management tool used throughout the project. I enjoyed using trello due to the intuitive features and the fact that it is a lightweight version of Jira that does not require as much configuration. 6 columns were created to track progress throughout the development process: backlog, to-do, in progress, testing, done and blocked. 

I created the following labels to categorise cards and increase productivity: planning, user stories, styling, bugs, features, development and documentation. I tried to provide an adequate amount of information on each card that provided a description and requirement where possible. 

Pomodoro timer was also used for timing tasks however I found this to be less effective due to unknown errors and issues that occurred during development. The time was useful for styling certain components and ensured I spent less time on how the application looks and more time on the functionality. 





