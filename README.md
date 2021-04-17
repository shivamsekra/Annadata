# Annadata-अन्नदाता(A Krishak Kalyan App)

![Capture1](https://user-images.githubusercontent.com/58334597/115112109-84b5f380-9fa1-11eb-84b2-c787ed1146ea.PNG)
      
 
# INTRODUCTION​
* There are many problems that a farmer faces during their day-to-day life. They are  not well educated and generally people like merchants take advantage of farmers and they often mislead them, for example, charging more money from the farmer than the actual rate, and   there are many such examples which suggest that the farmer in our country are taken advantage of. 
* They may not have proper knowledge of how market works or what seeds to sow at what time of the year.
* Keeping the above points in mind we have decided to help our farmers, by developing an app Annadata: A Krishak Kalyaan App
* It has been developed using latest technologies like ML and Data Analytics.
* It has an integrated platform which will cover up solutions for most of the problems faced by  farmers.
* Interface has been designed keeping in mind the education and skills of the farmer. So, that they can easily access our application.

Here, are some Scrrenshots form Application.

![Screenshot_20210417-180329_Expo Go](https://user-images.githubusercontent.com/58334597/115113680-1a08b600-9fa9-11eb-95a3-3d00ceca9c2e.jpg)
![Screenshot_20210417-180403_Expo Go](https://user-images.githubusercontent.com/58334597/115113730-5fc57e80-9fa9-11eb-83b0-3b2274fd1c6e.jpg)
![Screenshot_20210417-180411_Expo Go](https://user-images.githubusercontent.com/58334597/115113736-6227d880-9fa9-11eb-9e03-2b8b3e7b5545.jpg)
![Screenshot_20210417-180416_Expo Go](https://user-images.githubusercontent.com/58334597/115113737-63f19c00-9fa9-11eb-97d9-95280a383bde.jpg)
![Screenshot_20210417-180421_Expo Go](https://user-images.githubusercontent.com/58334597/115113741-648a3280-9fa9-11eb-9898-3574249c3180.jpg)
![Screenshot_20210417-180430_Expo Go](https://user-images.githubusercontent.com/58334597/115113908-46710200-9faa-11eb-9c66-f276eb77f9dc.jpg)


* APPLICATION DEMO
To take a demo please install Expo-Go application form play-store and scan this QR code from the app to access Annadata.

![expo](https://user-images.githubusercontent.com/58334597/115113271-22f88800-9fa7-11eb-9ca2-a4af145904f6.PNG)



# MOTIVATION​
Looking at the disturbing numbers of the suicides and due to the exploitation of the farmers we the team of Annadata thought of developing this application.​
Due to digitalization, there has been a steep reduction in the sales of local merchants, as they don’t have platform to sell their products online.​


# SCOPE OF THE PROJECT​
1. Prediction Of Harvest Yield Before Season
2. Crop Prediction
3. E-mart for Farmers
4. Government Schemes
5. Soil Quality Checks
6. Kisaan Calculator

# PROPOSED ARCHITECTURE​

![archi](https://user-images.githubusercontent.com/58334597/115112324-a9f73180-9fa2-11eb-9466-f490f204383f.PNG)

# TECHNOLOGY APPROACH

![tech](https://user-images.githubusercontent.com/58334597/115112332-b4b1c680-9fa2-11eb-9621-8b823a9e64b2.PNG)


# CROP YIELD PREDICTION - [AI-Feature-1]

This feature would help farmers to predict Yield in tons. We have taken data from different sources like data.gov.in / kaggle etc. 
After Feature selection and applying preprocessing techniques like handling null values, encoding etc we used following features.

![predict](https://user-images.githubusercontent.com/58334597/115112442-3a357680-9fa3-11eb-8448-51f13ca2a881.PNG)


ALGORITHM FOR CROP YIELD PREDICTION

-We worked upon multiple algorithms like xgBoost, RandomForest, NN, RNN-LSTM to achieve the best possible accuracy by comparing their Root Mean Square Values which after reading several research papers and comparing our results we found best to be used Random Forest Algorithm.

![code](https://user-images.githubusercontent.com/58334597/115112511-79fc5e00-9fa3-11eb-8414-ceeda1d89289.PNG)

RESULT ANALYSIS​

![result](https://user-images.githubusercontent.com/58334597/115112551-add78380-9fa3-11eb-9d6a-37bbb95ed7e8.PNG)


APP-INTEGRATION

![Screenshot_20210417-180437_Expo Go](https://user-images.githubusercontent.com/58334597/115113751-74a21200-9fa9-11eb-83d6-7dcf77ceacf6.jpg)
![Screenshot_20210417-182200_Expo Go](https://user-images.githubusercontent.com/58334597/115113890-2ccfba80-9faa-11eb-9491-f05c90fed65e.jpg)




# CROP PREDICTION - [AI-Feature-2]

This feature enables a farmer to predict what crops he/she can grow according to the type of soil.
This is an image classfication problem statement in which is trained on a dataset containing arounf 1000 images belonging to 4 classes i.e Alluvial,Red,Black,Clay soil.

We comapred VGG16, resnet50, mobile net v3 large and small. As all Are State of art algos , all were giving good accuracy of arounf 95%. 
Problem- As heroku provides only with 500mb so we decided to use small size model i.e MobileNetV3 Small without compromising any accuracy.

APP-INTEGRATION

![Screenshot_20210417-180444_Expo Go](https://user-images.githubusercontent.com/58334597/115113756-79ff5c80-9fa9-11eb-82ab-1efc5ff41d16.jpg)
![Screenshot_20210417-182125_Expo Go](https://user-images.githubusercontent.com/58334597/115113892-30fbd800-9faa-11eb-87ab-0ab3cf2f0d1f.jpg)



# E-Mart

Platform for Buy-Sell to help farmers cut mediator interests and provide farmer, households, merchnats with one single online platform for trade.


![emart](https://user-images.githubusercontent.com/58334597/115112797-d744df00-9fa4-11eb-9afe-024d0178ec49.PNG)


# GOVERNMENT SCHEMES​
We've scrapped data from The Economic Times website using Beautiful soup.

![gov](https://user-images.githubusercontent.com/58334597/115113105-293a3480-9fa6-11eb-8f9e-2df407eafc47.PNG)


# SOIL QUALITY CHECK​

Farmer can request for Soil quality check to get better insights and predictions on  basis of their soil type and quality.

![soil](https://user-images.githubusercontent.com/58334597/115113095-22132680-9fa6-11eb-9103-2b0e6921ada2.PNG)


# KISAAN CALCULATOR​
* Through this feature we are trying to make farmer aware​
* Farmers are being charged interests on the day basis.​
* We used Simple interest formula to calculate final amount.

![calci](https://user-images.githubusercontent.com/58334597/115113089-1b84af00-9fa6-11eb-8775-700a6384ebbf.PNG)


# BACK-END IMPLEMENTATION​
Backend implementation has been done by using online database i.e MongoDB Atlas. Database than has been connected to front-end using Flask App which is deployed on Heroku.

![mongo](https://user-images.githubusercontent.com/58334597/115113080-1162b080-9fa6-11eb-919b-ce27f11fee42.PNG)

![flask](https://user-images.githubusercontent.com/58334597/115113084-16276480-9fa6-11eb-8f9c-e95b3819c278.PNG)


# DEPLOYMENT-HEROKU​


![heroku](https://user-images.githubusercontent.com/58334597/115113069-0871df00-9fa6-11eb-867d-ede3f7d58de0.PNG)



# FUTURE WORK​

1. We will work on the efficiencies of the prediction and classification algorithms. ​
2. We plan to integrate soil quality check with crop prediction feature to give best AI based predictions.
3. Also, we will add the GPS feature in buy/sell section so that farmers can get local buyers/sellers easily.​
4. We will add new widgets and drop downs to make the app more efficient to use.​
5. Finally, we will also add some more regional languages in a planned manner so that users from other states can use it as well. 


# IMPACT​

1. Our application will indirectly focus on reducing the suicide rates of the farmers by increasing their Per Capita income.​
2. Our app will remove various barriers and hassle which farmers face while buying/selling various products related to farming.​
3. It will help them become more aware , organized through various features introduced in our application.​
4. For merchants also, it will cut their raw materials cost as there is no involvement of broker and it will give them various opportunities to expand their businesses by selling their products online to a massive population of farmers.


Members- https://github.com/Marmik343
