# Rainpower
Rainfall Calculator and Harvesting Tool
https://ddf46429.springboard.com/uploads/resources/1581702771_SEC_Capstone_Step_Two__Project_Proposal.pdf

1. Goal
The website will allow users to calculate rainfall estimates for their rainwater harvesting system. Users will be able to save "properties" that will have historical rainfall data. This data will be able to be viewed as daily, weekly, and monthly totals.


2. User Base
We expect our users to be homeowners, churches, and businesses that already use rainwater harvesting to supplement their water use. This app could also be used by a business in the rainwater harvesting industry as a incentive for customers.


3. Data
We plan to use both historical and forecast weather data via OpenWeatherAPI. Additionally, we may incorporate an API to estimate roof surface area from a given street address. 


4. Approach
We will start by creating a single page home page for all (non-logged-in users) that will take in a surface area measurement and a zip code. This will return a volume in liters/gallons. If possible, the user will be able to toggle between:
today, yesterday, last 7 days, last 30 days, next 7 days, and next 30 days.

For logged-in users, we will show this same split of data for their saved "properties". 

Database Tables:
User - (name, username, pwd)
Property - (surface area, zip code, user->User)
Day (Rainfall)

Security:
We will need to secure the user passwords
If we incorporate the roof surface area API, we will need to secure the proerty address.

In the future, we hope to make our app compatible with bluetooth/network enabled water gauges, so that users can see a real-time volume measurement for their harvested water.  
