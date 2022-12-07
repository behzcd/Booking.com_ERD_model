# Final Project
Final report

Group C:

Abdulaziz 12190257

Mukhammadsidik 12194846

Bakhodir 12194850

Bekhzodbek 12194852

Maftunakhon 12194847

DATABASE FINAL ASSIGNMENT
Professor Mehdi Pirahandeh
Designing and Implementing the script of a database for the Booking.com schema
 
Goals:

1. To gain experience implementing scripts for hotel management database
2. To gain experience designing Entity-Relationship (E-R) diagrams using ERWIN data modeler.
 
Task description:
 
   Online hotel booking provides hotel booking services to various travelers and visitors. It serves several customers. Each Hotel requires a modern database system for efficient management of its services and rooms. Our team is hired to design and develop a database that can meet the requirements of the hotel’s database management

Booking.com database requirements

All of the information related to the transactions that occur daily in each hotel database system is contained in the table named “Transactions”, which includes transaction id, payment id, customer id, extra charges id, transaction date, and transaction status.

The Hotel’s detailed information about its id. Hotel name owner’s first and last name, contact number, and email is provided in the table named “Hotel”

“Locations” table is used to provide to give address information, street, city, country, zip code, latitude, and longitude.
 
The “Payment” table includes extra charges id, customer id, payment type, currency, currency image, payment date, payment status. 

“Extra charge” table used for, if customer brake down any item by using name, cost and description.

Customer table provide first and last name, street address, city, country, zip code, birthday, contact number, email, language id.

“Reservation” table: The data in this table pertains to each reservation a client makes or that a front desk agent executes. This table stores the data of hotel id, customer id, room id, transection id, reservation id, check in, check out, no of guests, smoking and pets id. 

The “Rooms” table records all different room information in hotels with the variables including room id, roomtype id, status id, room number, room picture, overall price. 

The table “Room type” stores all of the room kinds by using roomtype id, room name, description, max guests, smoking, pets, room price (USD) functions as well as their additional characteristics if any.

The “Room Status” table shows if the room is occupied, unoccupied, or in the process of being cleaned by using function dependence of status id, status name, status description.  

One of the tables is called “Hotel overview” that related directly to hotel to give information of satisfaction by using following functions, they are hotel rating, imaged id as a foreign key and hotel id.

Next table is “Hotel image” related to “Hotel overview” that table provide the hotel images to show hotel to other customers. This function work by uploading image and use added by and added at functions and its status too. 

To make convenience to customer the is “Discount” table that use discount id, hotel id customer id as foreign key and discount type, description, and promocode.

“Recommendations” table that match best fit of hotels to customers by using the functions of recommendation id, customer id, top hotels, and options of choosing low-price, best by search, best by rating, best by promotions, best by roomtype, best by recommend.

“Feedback” is another table that customer can give feedback about hotel experience, for that use feedback id, hotel id, customer id as foreign key and feedback type, feedback itself, feedback data and rating 5 stars.

“Settings” table related to “Customer” table and use settings id, customer id and language id as foreign key. Also, it can be used for editing profile, notification, privacy security, advanced settings, contact customer service, how to use and FAQ functions.

“Login” table, Customers can login to the webpage and will have name, password and of course information about the date they login.

“Language” table. Staff of the hotels should have their name written on the table and their language and this table is linked with the language table which has language name and ISO code.

“Hotel staff” table contains staff name, staff language, and its language id.

“Report” table. Customers can report if there are problems related to anything in the hotel. If something is broken for example the system will have info of the report type, report, report date and report status (whether solved or not.)

“Search” table Customers can also search hotels based on the country, city, and even hotel name, or room type they would like, and can filter the price they want or even search for discounts, and in the web page the rating of the hotel is visual, and client may see the pictures of the hotel based on their search.

ERD Model also contains info related to the admins and there is a separate ERD table for it. It has following inputs:

The “Admin” table that contains Admins name, username, password, address, contact number and email.

The “Settings” table contains admin id as a foreign key and menu, data rows, display name, description, icons, and servers.

The “Activity” table includes admin id, customer id, type of the activity, description, and activity date.

The last table named “History” stores info such as admin id, customer id, activity type, created by, created on, updated by, updated on, deleted by and of course as required deleted 




![image](https://user-images.githubusercontent.com/114143258/206217088-f439baf9-4104-4b84-924f-37386911e26f.png)




Firstly, we have created ERD diagram according to task requirements:

![image](https://user-images.githubusercontent.com/114143258/206217206-1df551a3-ef37-4187-94ec-e383933f4f77.png)

 
       One of the main tables in our ERD is hotels, because booking website work between customer and hotels. Hotels table include information about hotel that customer wants to visit, and it contain hotel name location id overview id owner first and last name contact number and email box. Here first related table is location. In location table we use the information of address, street, city, country, zip code, latitude, longitude. To choose hotel most customer try to quick overview, and here we use hotel overview table to give information about hotel rating and image id. In that table, there is hotel images, including images, added by, added at, status.
 
 ![image](https://user-images.githubusercontent.com/114143258/206217267-d5789839-f233-4fe4-8bfd-b1f7602579b5.png)
![image](https://user-images.githubusercontent.com/114143258/206217309-259eac7c-d11c-42dd-bb52-49964f65e1cb.png)
![image](https://user-images.githubusercontent.com/114143258/206217361-9899ce9a-93ed-43e3-bbe3-22c8694a73fe.png)
![image](https://user-images.githubusercontent.com/114143258/206217457-99726e67-a501-46ac-9952-d7f33e865ad5.png)
![image](https://user-images.githubusercontent.com/114143258/206217603-2415c2f6-4049-4bcf-9933-fa7483d95cbe.png)

 
        Each reservation that a guest makes or that a front desk agent completes is recorded in the hotel's "Reservations" database. This table keeps track of data such the reservation id, check-in and check-out dates, guest count, room id, customer id, and transaction id as functional dependencies. The "Room" table uses the variables room type id, room number, floor num, and status id to keep track of all the various room-related information for each hotel. The "Room type" table uses the room type id, room name, maximum number of guests, smoking availability, description, room cost (USD), and, if relevant, any additional characteristics to keep track of all the various room kinds. The "Room Status" table displays whether a room is inhabited, unoccupied, or being cleaned based on the function dependence of status id, status name, and status description.
 
 ![image](https://user-images.githubusercontent.com/114143258/206217681-3acaf124-5d61-4a33-9dfa-6ea27ecb5893.png)
![image](https://user-images.githubusercontent.com/114143258/206217715-2498cf2d-1fd0-450d-aa58-1b7155125589.png)
![image](https://user-images.githubusercontent.com/114143258/206217744-7f964829-647f-44e9-9b30-bc60782ea223.png)
![image](https://user-images.githubusercontent.com/114143258/206217795-1c01e863-7dc0-4620-a2a9-f161c190e8e1.png)

 
 
 ![image](https://user-images.githubusercontent.com/114143258/206218113-1b0251a1-8608-4cca-8999-a57f5bf8c6ee.png)


     All the information related to the transactions that occur daily in Booking.com database system is stored in the table named “Transactions”, which includes transaction id, customer id, payment id, extra charge id transaction date and transaction status. There is customer table that save all personal information about booking.com customers, their first and last name birthday, contact number and email, address related information, for example street, city, country and zip code, and acceptable language too. These two-table related to payment to make payment online through website. Here, we use payment id and extra charge id if there was and customer id, payment type, currency according to visa or master card, currency image, payment data and payment status. Extra charges only used when customer breaks down something like dish or furniture. We use name of broken item, its cost and description. And last table related to transaction is reservation to match customer and hotel in advance after customer choosing appropriate hotel. There is hotel id, customer id room id or number, check in and check out for payment number of guests for single or multiple people room smoking or non-smoking inside room and pets’ allowance.
 
 
 
 

 


      As we explained customer table above it saves customer personal information. There are settings that include customer information and additional functions to make convenience to customer. Customer can edit profile use notifications, privacy, and security of customer service, how to use, FAQ and language too. For the language table we created functions by naming languages by typing or ISO code to find by scrolling. And this table matches customer to hotel staff who know the language that customer choose as his or her first or acceptable language. And customer can see staff name, staff language by choosing appropriate language.
 


 
     To being familiar with customer and hotels table. In this picture few more related tables too. One is recommendations to recommend and best match customer and hotels. There are top hotels, low price options and best by search, best by rating, best by promoting, best by roomtype, best by recommend functions. Next is discount table for customers using hotels and customer ids and with the information and function of discount type, description, and promocode. To make convenience to customer to search, there is search table that includes search by country, search by city, search by hotelname, search by roomtype, search by price, search by discount, search by rating, search by images functions. Feedback table is created to write feedback after using hotel to give information about hotel including feedback type, feedback itself, feedback date and 5 stars rating functions. If there is any problem using hotel, with the information of report type, report, report date, report status. Last table is login for customers with the functions of username, password, login date.
 

 
      Lastly, we created “Admin” table that contains Admins name, username, password, address, contact number and email. Also, the “Settings” table contains admin id as a foreign key and menu, data rows, display name, description, icons, and servers. Followd by the “Activity” table includes admin id, customer id, type of the activity, description, and activity date. The last table that we inserted is named “History” stores info such as admin id, customer id, activity type, created by, created on, updated by, updated on, deleted by and of course as required deleted on.
 

       In the Collab, we imported two things as written in the code and connected it to the database. And inputting the data as follows.
 
         For other data also, we used the same procedure, and you can see the whole code by just clicking the link below. (Since google Collab doesn’t support foreign keys and primary key we constrained to display these things.)
The assignment was done by each member of the group but uploaded only by one person. Thanks for your attention.
Here is the link for the code in GitHub https://github.com/bmukhammadaliev/Final-Project/blob/8f93df9e212e0c072b3eaa1b51642ca0f75ab7cb/Hotel.ipynb 





