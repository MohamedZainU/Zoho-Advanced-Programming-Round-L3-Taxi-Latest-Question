# Zoho-Advanced-Programming-Round-L3-Taxi-Latest-Question
Low Level System Design for Taxi Booking Latest Zoho L3 Question



Remember all the Details will be given by them the taxi,customers and Admin details our task is to assign nearest taxi to the customers only the given taxi should be allocated repeatetively no taxi should be created newly other than the question given same applies for Customers and Admin for Admin 1 can only be the Admin and Admin will get 30% commission for each ride from the Driver 

for eaxmple nearest Taxi what i mean is

Taxi ID 4 current Spot is A
Taxi ID 2 current Spot is C
Taxi ID 3 current Spot is E

Customer Books Taxi:

pickup is A 

drop   is B

then we need to find the Taxi ID which current Spot is nearest to A 

for this case 

Taxi ID 4 current Spot is A then Taxi 4 can be allocated

Taxi ID 4 is alloted

Now Another Case 

Now again the Customer books Taxi 

now Taxi 4 is currently in B cause from A it moved to B cause of drop Location change

Customer Books Taxi:

pickup location is B too

and Drop is E

Taxi ID 4 current Spot is B
Taxi ID 2 current Spot is C
Taxi ID 3 current Spot is E


In that case we should Assign Taxi to Taxi ID 2 cause we should give the allocated Taxi 4 a rest for once

So now the nearest for pickup B is Taxi 2 which is in C

Now Again the Customer Books Taxi 

pickup is B

drop   is D

Updated Taxi Positions
Taxi ID 4 current Spot is B
Taxi ID 2 current Spot is E -> changed
Taxi ID 3 current Spot is E

Now we can assign Taxi 4 cause we gave Taxi 4 rest once so yeah



1. You will be given 4 Taxi for that 4 Taxi each Taxi will be provided with ID and current Spot

Taxi t1 = new Taxi(1,'D');
Taxi t2 = new Taxi(2,'B');
Taxi t3 = new Taxi(3,'G');
Taxi t4 = new Taxi(4,'A');

the above 1,2,3,4 represents their ID and Characters represents their current spot

2. You will be given 2 customers for that 2 Customers each Customer will be provided with name and password

Customer c1 = new Customer("aaa",134);
Customer c2 = new Customer("bbb",124);

the String represents name and integer represents password

if you don't understand this see Taxi class Constructor and Customer class Constructor


3. You will be given 1 Admin for admin same name and passwd will be given

Administrator admin = new Administrator("ZULA",1354);

4. You have check if name and passwd matches for Customer

then now you can book Taxi


