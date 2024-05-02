# This is MTI University's Final Project (Web-Application-for-Medical-Care-Services -- MediCarePlus --) hospital room reservation part is taken from the hospital room reservation system Mohammed Sameh's Final Project to cs50 
### Programming languages Used: HTML & CSS, JavaScript, Python (Flask), SQL
### Libraries and frameworks used : Flask, Flask-session, Jinja2, Werkzeug, pytz, requests, sqlite3

# Description:
### This web app is a medical care services web in which it's main purpose is to simulate schedule appointments, room reservation , adding users with different roles and different system functions accuses and generating reports as similar as real hospital medical web-baised system.


### 1. The user can sign in himself/herself by providing his details (username & password).
### 2. After signing in the user will be redirected to Main page where he/she has options that's differs according to user's Role

## Disclaimer Alert: gifs design that explain rules and functions are a old versions of design but still have the same functions without any changes changing web design is not finished yet
### logo is changed from Al salam hospital to MediCarePlus
![MediCarePluslogo](logo.png)
## Icon
![MediCarePluslogo](favicon.ico)

for example:

### <h1>1. Admins:</h1>
![Admins](gifs/david%20admin.gif)

<h2>Admins can do:</h2>
    <ol style ="font-size: 14pt;">
        <li>Adding new users all roles (except admin which they are added by default in database).</li>
        <li>Changing users status from working to ("Fired","Retired","Moved","Promoted","Demoted","Transferred") or 
    vice versa (except admins which there statuses is determined by default in users tables).</li>
        <li>Patient registration.</li>
        <li>Book a room for patient after patient registration.</li>
        <li>Check out a reservation</li>
        <li>Able to see users actions report and print it</li>
        <li>Able to check rooms (room no., price, status) and print it</li>
        <li>Able to see reservations history and print it</li>
    </ol>


### <h1>3. Receptionist:</h1>
![Receptionist](gifs/Receptionist.gif)

<h2> Hospital Receptionists can do:</h2>
    <ol style ="font-size: 14pt;">
        <li>Patient registration.</li>
        <li>Book a room for patient after patient registration.</li>
        <li>Check out a reservation</li>
        <li>Able to check rooms (room no., price, status) and print it</li>
        <li>Able to see reservations history and print it</li>
    </ol>

## Disclaimer Alert: this part is still not finished yet so the part won't be providing a graphical representation as an explanation of users's capabilities (aka: functions)
## Important Alert: Clinic is a newly added part that comes from the use case of the user (clinic receptionist) that is been done by Salma Assem in association with Prof. DR. Noha Mohammed and Team leader Mohammed Sameh
![clinic receptionist](Screenshot_20240503_012021.png)

<h2> Clinic Receptionists can do:</h2>
    <ol style ="font-size: 14pt;">
        <li>Book appointment for patent to clinic visit to doctor</li>
    </ol>
<mark style = "background-color:Green; font-size: 24pt; color: white;">All Users usernames, passwords,role and status in users.txt</mark>

## page :

### 1. Patient Registration
![Patient Registration](gifs/patient%20regestration.gif)

<p>Patient registration allow to users to add patient personal information, Contact information And Emergency Contact Information</p>

### 2. Check In
![Check In](gifs/check%20in.gif)

<p>Check in comes after patient registration which in this page users select patient data and room that are available to him/her, each room selection has a price , check in date and check out date having a minimum value of today and payment method (Cash, Visa or Mastercard).
After check in the room status change from open to reserved</p>

### 3. Check Out
![Check Out](gifs/check%20out.gif)

<p>Choosing a reservation to add an exit date to this reservation (N.B: exit date is the real date with the patient left the hospital).
After check out the room status change back to open and become available to be reserved agin in check in.</p>

![Check Out](gifs/reservations%20history2.gif)

### 4. Employees Report
![Employees Report](gifs/users%20report.gif)

<p>This page shows the users information of like name, there roles in system, there status, and no. of reservations made by users (For reporters no. of reservations is none) and any actions notes.
And user can Print this report by clicking button "print this page".</p>

### 5. Add New User
![Add New User](gifs/Adding%20user.gif)

<p>This function is available to only admins and reception manager which:
<strong>Admin can add only reception manger, receptionist and reporter</strong>
<strong>Reception manager can only add receptionist </strong>
Once user is added he/she can use system in restricted borders</p>

### 6. Changing User Status
![Changing User Status](gifs/changing%20user%20status.gif)

<p>This function is available to only admins and reception manager which:
<strong>Admin can change status to only reception manger, receptionist and reporter from from working to ("Fired","Retired","Moved","Promoted","Demoted","Transferred") or vice versa .</strong>
<strong>Reception manager can only change status to receptionist from working to ("Fired","Retired","Moved","Promoted","Demoted","Transferred") or vice versa .</strong>
Once the user's status changed from working to anything else he can't use the system and vice versa. </p>

![Changing User Status](gifs/users%20report2.gif)

### 7. Check Rooms
![Check Rooms](gifs/check%20rooms.gif) 

<p>This page shows rooms information: room no, price and status which it can be "open","reserved"
And user can Print this report by clicking button "print this page".</p>


### 8. Reservations History
![Reservations History](gifs/reservations%20history.gif) 

<p>This page shows Reservations information: Rooms No.	patient Name, Check In Date, Check Out Date, Exit Date, Total Price, which is no of reservation days * price,....etc. .
And user can Print this report by clicking button "print this page".</p>

## Disclaimer Alert: this part is still not finished yet so the part won't be providing a graphical representation as an explanation of users's capabilities (aka: functions)
### 9. Schedule appointments


<p>This page takes clinic patient's appointment information: patient Name, Appointment Date, hour, clinic name ,doctor name, email </p>
