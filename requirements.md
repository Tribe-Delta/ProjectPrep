# Project Requirements

## What is the vision of this product?

- To both inform and prepare travelers before they arrive at their desired locations with information about their trip.

## What pain point does this project solve?

- It gathers useful information and aggregates it in one area for instant and easy referencing

## Why should we care about your product?

- Because being an informed traveler makes you more accessible to the local culture and people

## Minimum Viable Product vs Stretch

- What will your MVP functionality be?
  - Multiple Location Search
  - Map
  - Notes
  - Plug Adapter
  - Exchange Rate
  - Auth0 authorization

## What stretch goals are you going to aim for?
- “Things to do” feature

## Functional Requirements
List the functionality of your product. This will consist of tasks such as the following:
1. An admin can create and delete user accounts
2. A user can update their profile information
3. A user can search all of the products in the inventory

## Data Flow
When a user arrives at the site they will be required to login with their credentials or sign up for a user account.  
After authentication a user will then be prompted with a form field requesting a city name the user intends to travel  
to. The user can then search for just the one location, or add multiple locations to their search depending on their  
needs. After submitting the form, results will be displayed showing a general map of the location, currency information,  
flag, coat of arms, language spoken, exchange rate, power adapter, lat and lng and possibly things to do in the area.  
Each location searched will have an option for adding notes such as what to bring, who's traveling with them, etc.  
Searches and notes can then be saved as a “trip” via a save button. This data can then be revisited by the user at any time.  
Entries can also be manually deleted at any time. Last of all a user can leave the page or log out at any time however if  
they have no saved results they will not be added to the database.

## Non-Functional Requirements (301 & 401 only)
Non-functional requirements are requirements that are not directly related to the functionality of the application but still important to the app.

1. Security:
   - Users will use Auth0 to log in to the site. 
   - Verify that uses have valid email addresses and aren’t bots trying to destroy Dan’s credit

2. Usability	
   - The site will contain a single field in which the user will enter a city.
   - They will press a button to send the request to get information on that city
   - They will be shown a field with information about that city
   - We will strive to make this site accessible to screen readers

3. Error codes
   - The site will display error codes if the user runs into an error while trying to access the site. This will allow users to understand  
   why their search did not return the result they had hoped for.
   - On the development side there will be error codes for us to help us understand where our program goes awry
