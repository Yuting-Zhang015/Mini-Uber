## Instructions of using RIDE web application
Author: Yuting Zhang(yz579), Huiling Yan(hy165)
Develop tool: Django

Thanks for using RIDE. In this README file, we'll show you through our rideShare app. In the up navigation bar,
you can click home to go back to this user home page whenever you want, you 
can click on the Login/Logout button whenever you want, also you can click on the profile to see your informaion.
The profile will show your user information, after you registered as a driver, the profile will include your car informaion.

## Login Page
When you successfully connect to the server, you shall see a login page. For the
ones who does not have an account yet, you should click on the Sign up now 
button on the bottom right to sign up for an account.

In our user register page, you shall see several columns: Username, Email, 
password and password confirmation. On the right are some help-texts to inform 
you the format of the columns. Note that for the email column, you should enter
an valid email address, otherwise it will pop up an error message. Also for
the password, you should enter exactly the same string, or it will remind you
that two passwords don't match. After you sign up, it will lead you to the login
Page where you can login, after you login you will see the user home page.

## User Home Page
There are 6 titles indicate different functions. Their specific functions and the design details are 
described below.

### View Open and Confirmed Rides
When you click on it, you shall be redirected to a page, listing all the open and 
confirmed rides that belong to you. They're ordered by the arrival time, and 
indicated by destination address and ride status. 
When you click on a paticular ride, you shall see the detail of this very ride.
It is composed of two parts, all ride details and driver information. For open rides,
it only shows ride details without driver information; after a driver confirms it, 
the ride status will be changed to confirmed and driver information will be shown below.
Besides, the ride detail will not include sharer information before a sharer join the ride.
If the ride has both owner and sharer, the sharer information will be added to the ride information.

### Edit Open Rides(as owner)/View Open Rides(as sharer)
This page lists out all of your OPEN rides, both as a owner and as a sharer. Every 
ride is clickable, you can look into it and view the detail.The diference between 
owner and sharer is that when you're an owner of this ride, you are able to edit 
the ride information by clicking 'edit' button, and the page has a title "Edit the
ride information"; however for sharers, you're not allowed to edit the information,
the page has no edit button, and the page has a title "View the ride information"

### Request a ride
This page is for requesting a ride as owner. When you click on it, it shows a form,
and you should fill out the required information. Note that the last two columns
(Vehicle Type and Special Requirement)are optional, you are free to leave it blank.
The owner name is the username of current log-in user by default, and *you should
not change it*. Then fill out your destination address, arrival time, passenger
number and sharing status (if you would like to share this ride or not), and then
click 'Request'. Now if you go back to the user's home page and click on 'View 
Open and Confirmed Rides', you shall see the ride you just requested as well as
the detail you've just filled out.

### Join a ride
Here you can search for a ride to share as a sharer. Fill out your destination,
anticipated start arrival time and end time, as well as the passenger number, 
it will show you the current available ride to share and its details. In our design,
if no ride meet the search requirment, the page will show a message "Currently no rides available."
If there are one avalible ride that meets your requirement, the page will jump to this rids's detail
page and ask if you want to join the ride. If you do want to join this ride, fill out the passenge number.
The user name field is the username of current log-in user by default, and *you should
not change it*. After fill out the information, you can click the join button to join the ride. Then
the page will jump back to the user home page. Now if you click "view open and confirmed ride",
you shall see the ride you just requested as well as the detail you've just filled out since you
joined the ride just now.

### Register as driver
A logged-in user can register as a driver through this link. After you click this link, it shows you
a form to fill out your car information. Note that the last column (Special vehical information) is optional,
you are free to leave it blank. After you register, you will be lead to "As a driver" page, you can click the 
home button on navigation bar to go back to User Home Page any time you want.

### As a Driver
If you have not registered as a driver before, this page will just shows the message 
"Please register as a driver first!".  If you go back and registerd as a driver, you will see
a page shows two options.:

+ "search for open rides": when you click this link, you can see a list of open rides, each ride is clickable.
The driver cannot see the open ride created by herself/himself. If you want to confirm a ride, 
you can click the ride to edit its status from open to confirmed. You can see your username on this
page, please not change it. Now it will lead you to the page "view my confirmed page". You can view your confirmed rides here.

+ "view my confirmed page": if you are a driver, this page shows you all confirmed rides belongs to you.
After you have finished a ride, you can click this ride to edit the status from confirmed to completed.




















