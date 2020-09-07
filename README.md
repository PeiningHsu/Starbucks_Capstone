# Introduction

This is my capstone project for Udaciry Scientist Nano Degree. I will use the skills I have learned in this class to analyze the data and build model.

# Motivation
 
Starbucks is a world-wide known coffeehouse. It has many promotion events and even has it's own app by which the members can receive the latest promotion information. There are many other local coffee shops or even other chain coffee stores where Starbucks locate. Therefore, Starbucks have to do marketing strategy to increase their revenue and compete with the rivals. I am interested in discovering actionable business strategy and improving current strategies. Hence, I will provide the suggestions to Starbucks which might help them to improve their promotion results. 

# Libraries used

Pandas  
Numpy  
Matplotlib.pyplot  
Sklearn  

# Files in the repositories

portfolio.json  

id (string) - offer id  
offer_type (string) - type of offer ie BOGO, discount, informational  
difficulty (int) - minimum required spend to complete an offer  
reward (int) - reward given for completing an offer  
duration (int) - time for offer to be open, in days  
channels (list of strings) - by which Starbucks send out the offers: email, web, social, mobile  

profile.json  

age (int) - age of the customer  
became_member_on (int) - date when customer created an app account  
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)  
id (str) - customer id  
income (float) - customer's income  

transcript.json  

event (str) - members' action to the offers:  offer received, offer viewed, transaction(members responded but not yet complete), offer completed  
person (str) - customer id  
time (int) - time in hours since start of test. The data begins at time t=0  
value - (dict of strings) - either an offer id or transaction amount depending on the record   

# Summary

We have more male members. However, members of different gender have similar response rate, which are about 0.61. Even though, male have lowest complete rate, which is only 0.106, female 0.137, and others 0.128.

People complete more discount offers than bogo offers. However, we cannot conclud that people less respond to Bogo as we don't have the offer type for those offers in transaction status. It might be possible that people do respond to Bogo but are unable to complete it in time.

Interestingly, more than 50% offer 5 are not reviewed but given it is reviewed, more than 60% will it be completed. Offer 5 are distributed by web and email. It might be the reason that people don't open the offers. 

Offer type doesn't change much throughout the different age. However, people in young age respond to the offer most actually, then older people. People in middle age respond less actively. One possible reason might be that people within age 35-55 are too busy to respond to the offers. For younger and older people, they might have time to respond to the offers. The other possible reason is that people in middle age are not sensitive to discount/promotion. People under 35 have more than 60% to the offers. People over 55 have second response rate and the people aged between 35-55 have the lowest response rate.

In addiiton, people will view Bogo offers more than discount offers but complete less to Bogo given they reviewed it. However, we can not find the reason for the phenomenon as we currently don't analyze the offers of transaction status. If we can get the data for transaction, we can check if people do responde to Bogo but are unable to complete it. However, if it turns out that people do view more bogo but respond less, we can do some test to see why. It might be the reason that the content/layout of the offer information is not attractive. We can use A/B testing to see if a new version or new design of the offer content/layout will attract people to respond more. I look deeply into bogo offers and discover that people complete offer 4 7% higher than offer 1 and 2, 4.5% higher than offer 9. The reason might be that the difficulty of offer 4,which is 5, is the least and duration, 7, is longer compared offer 9 which is also difficulty 5 but duration only 5. In my opinion, the reason why people view more Bogo but don't complete it is because that they view the offers to see if they are type 4. If the Bogo is type 1 or 2, then the members probably won't respond. 

In addiiton, people will view Bogo offers more than discount offers but complete less to Bogo given they reviewed it. However, we can not find the reason for the phenomenon as we currently don't analyze the offers of transaction status. If we can get the data for transaction, we can check if people do responde to Bogo but are unable to complete it. However, if it turns out that people do view more bogo but respond less, we can do some test to see why. It might be the reason that the content/layout of the offer information is not attractive. We can use A/B testing to see if a new version or new design of the offer content/layout will attract people to respond more. I look deeply into bogo offers and discover that people complete offer 4 7% higher than offer 1 and 2, 4.5% higher than offer 9. The reason might be that the difficulty of offer 4,which is 5, is the least and duration, 7, is longer compared offer 9 which is also difficulty 5 but duration only 5. In my opinion, the reason why people view more Bogo but don't complete it is because that they view the offers to see if they are type 4. If the Bogo is type 1 or 2, then the members probably won't respond.

There are some data which can improve my analysis, and I also believe these data are available in Starbucks database. Besides, supposed I can get those data and analyze the results, I will design some A/B testing to figure out the exactly factors that drive members to respond the offers.
