# e-commerce

## Content
- [Project Description](#project-description)
- [Project Goal](#project-goal)
- [Thought process](#thought-process)
- [A step-by-step approach](#a-step-by-step-approach)
- [Visualization](#visualization)
- [Dataset](#dataset)

## Project Description  
The project intends to explore the user behaviour of a C2C fashion platform and to make data-driven recommendations to improve the overall growth of the platform.

## Project Goal
The goal of this project is to practice creating and interpreting different types of visualizations using real world data.

## Thought process
The original idea was to find real world data from an e-commerce business. A dataset of over 95k users of a French C2C fashion store was found on Kaggle that showed interesting metrics, such as number of products bought/sold, last days since last login, operating system used, countries, etc. from which compelling visualizations and relevant recommendations could be derived.

## A step-by-step approach
The dataset contains data from ca. **95k users** of a C2C fashion platform (i.e. Kleiderkreisel / Kleinanzeigen alike) with information on: country, language, gender, number of products sold by user, number of products bought by user, number of users who follow user's activity, number of user accounts user follows, number of products listed by user, number of products in user's wishlist, number of products liked by user, days since last login, operating system used, etc.

First a cleaning of the dataset was conducted. During this process, only active users of the platform were kept for further analysis and visualization. Users were deemed to be active if they fell into one of the following categories:
- Exclusive buyers: users who have bought at least 1 product but haven't sold anything
- Exclusive sellers: users who have sold at least 1 product but haven't bought anything
- Both buyers and sellers: users who have bought at least 1 product and sold at least 1 product
- Prospective users: users who haven't bought and sold anything but who are actively interacting with other accounts
By segmenting the users into 4 groups, we hoped to bring to light specific user behaviours from which we could derive actionable insights to improve the overall growth of the platform.

The correlation between the different metrics were analyzed and visualized on Tableau and python with scatter plots, histograms, box plots and bar graphs: ([Notebooks](https://github.com/jsialell/e-commerce/Notebooks), [Tableau](https://github.com/jsialell/e-commerce/Presentation/Project_curry_visualizations_tableau.pdf)).  

### The following observations and actionable insights were made:
#### Expansion of Market Share:

##### Android targeted social network marketing campaigns
The amount of active users within the economically active groups are distributed unevenly. Android users only account for **7%** in those groups. For this reason, and due to the fact, that the average amount purchased and sold per Android user is on par with the iOS counter part, we advise to target Android users on relevant social networks. These focus mainly on social networks with younger people and a possible fashion affinity such as Instagram and TikTok. 

##### Browser QoL updates and screen real estate utlization
Lastly, within the same distributions, we see a large discrepancy with the Browser users, these are the largest user group, however have the lowest sales and purchases per user. For this reason it is highly advised to make the user experience comparable to the mobile intuitiveness with regards to selling - We recommend a iCloud and Google Pictures integration, bridging the gap between the accessibility of a smart phone and computer, with no viable camera option. To improve the purchasing power of the Browser group, we advise to make use of the extra screen real estate on a computer and add an upselling product recommendation addition.

#### Retention of User Segments:
##### Incentivize the first sale for single time buyers

The retention of the various user groups differ immensely. The most retained group are users purchasing and selling products. These users interact with the platform in a bilateral way, enabling maximum usefullness as they are involved in both the buyer and seller journeys. 

The group with the lowest retention is also the largest distributed group of users - the exclusive buyers. These have an average last login day of around 130 days before the data collection. In order to activate these users, it is essential to promote the exclusive, single time buyers an option to enter the seller journey without the high hurdle rate it usually encompasses. This can be done cost effectively via a voucher for a premium listing after any user completes their first purchase. 
A voucher would enable the user to consider selling, enjoying a higher success rate in their journey and mainly the introduction to it - allowing them to continue selling after their first successful sale.

##### Enable users to have their own social content page

There is a positive correlation between the number of social followers and the number of products sold by a user. Since having more followers helps users to sell more. The C2C platform should allow sellers to get more followers and more visibility. Our recommendation here is to empower sellers and provide them with their own personal user page on the platform where they can create attractive content and brand themselves. The platform should also increase its social integration, e.g. by offering a follow button for example on the user page.
##### Allow business accounts, with higher functionality 

The platform is significantly dependent on its top sellers: the top 1% of the sellers (20 top sellers) account for 17% of the total products sold, while the top 10% of the sellers (203 top sellers) account for ca. 60% of the total products sold. Considering the retention of the different user segments and their share in the number of products sold, we could see that there were two distincts groups of users on the platform: 1. private users with little product volume and activity and, 2. professional users with higher product volume and activity on the platform. Hence, the platform should better fit the needs of these two specific group. To do so, a subscription premium account for professional users could be considered. The premium account would allow users to customize their user page (styles, HTML) and better brand themselves. It would also offer premium listings.

## Visualization
- [Presentation](https://github.com/jsialell/e-commerce/Presentation/Curry%20Consulting.pdf)
- [Tableau Visualization](https://github.com/jsialell/e-commerce/Presentation/Project_curry_visualizations_tableau.pdf) 

## Dataset  
[E-commerce - Users of a French C2C fashion store](https://www.kaggle.com/jmmvutu/ecommerce-users-of-a-french-c2c-fashion-store/data) 
 
