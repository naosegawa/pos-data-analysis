# Analysis ideas
## 1. Predict number of units to be sold for each menu item  
### Goal
By offering predictions of how many units to be sold that day for each menu item, stores could estimate required inventory level better (or automate the order if the model is good enough), and hence minimize wastage.  
### Dependent variable
number of units sold for each item  
### Independent variables candidates
- weather (more likely to go to the store when it's not raining? would the sales gap filled by delivery sales?)
- date (store is likely to sell more if it's payday?)
- day of the week (more sales on weekend?)
- month (more sales in December?)
- holiday (more sales on holidays. which holiday sells more?)  

### Notes
- what drives the sales up/down?
- each item's proportion in sales is somewhat consistent?  
If yes: dependent variable could be just total number of items sold per day, and proportionately devide them for each item
- unless I include geographical features, I probably need to create multiple models for each store

## 2. Predict number of customers
### Goal
Prediction of number of customers for a particular day and time allows stores to assign optimal number of staffs in the shifts. 
### Dependent variable
Number of customers
### Independent variable candidates
- weather
- date
- day of the week
- month
- holiday
- time (more people during lunch and dinner time? trend changes on weekend and holidays?)

## 3. Detect suspicious transaction
### Goal
Detect suspicious transactions and prevent fraud caused by staff.
### Dependent variable
Confidence level for the transaction to be fraud.
### Independent variables candidates  
- gross sales per transaction
- spending per person (how far from the average?)
- length of stay (suspicious if it's too short but not take-out?)