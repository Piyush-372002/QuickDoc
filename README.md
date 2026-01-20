# QUICKDOC 

QuickDoc is a website that connects doctors, patients, and ambulance providers. Patients can select a date and doctor to consult, and the system will automatically generate an appointment time based on the doctor's schedule. Patients can also view their current and past appointments and book ambulance services. Doctors can accept or reject appointments, view all their current and past appointments, and upload detailed prescriptions for patients.

<br>

## Visit Online 🔗

This website is hosted at: https://quickdoc-1.onrender.com/

<br>

## Tech Stack Used

### 1. Backend
Node.js, Express.js

### 2. Database
MongoDB

### 3. Frontend
EJS Templates including HTML, CSS, and embedded Javascript

### 4. Payment Integration
Using Razorpay

<br>

## Figma Link for UI

https://www.figma.com/design/sFgEgANYz2W3bKXpQ5coME/Untitled?node-id=0-1&t=oTAfsw1g8EpVJg40-1

<br>

## Test Case Documentation

## 1. Manual UI Test Cases
<br>

| ID           | Title                        | Steps                                                                                     | Expected Result                    |
| ------------ | ---------------------------- | ----------------------------------------------------------------------------------------- | ---------------------------------- |
| TC_LOGIN_001 | Login with valid credentials | 1. Open app in browser 2. Go to Login page 3. Enter valid email & pass 4. Submit          | Dashboard loads & shows user info  |
| TC_LOGIN_002 | Login with invalid password  | 1. Go to Login page 2. Valid email + wrong pass 3. Submit                                 | Error: “Invalid credentials” shown |
| TC_LOGIN_003 | Login with empty fields      | 1. Submit login form with blanks                                                          | Validation errors displayed        |

<br>

## Screenshots for above test cases

<br>

<img width="1875" height="824" alt="image" src="https://github.com/user-attachments/assets/567a3bda-0ec2-4cec-8b16-cfc174e341ef" />

<br>
<br>

<img width="1862" height="831" alt="image" src="https://github.com/user-attachments/assets/95ba4bc6-5aa5-4f05-98d3-34505551f970" />

<br>
<br>

## 2. Automated test cases

<br>

| ID              | API                            | Payload                           | Expected                         |
| --------------- | -----------------------------  | --------------------------------- | -------------------------------- |
| PAYMENT_DOC_001 | `/patienthome/bookappointment` | `{doctor, specialty, date, slot}` | Razorpay Payment Interface opens |

<br>

## Screenshots for above test cases

<br>

<img width="1258" height="581" alt="image" src="https://github.com/user-attachments/assets/9a3e9f82-d91b-4ffc-b183-00193b9430e6" />


<br>
<br>

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Your machine should have Npm(or Yarn), Node.js, and MongoDB installed to use it locally.

<br>

## Setup and Installation

### Setting up the repository locally

1. First fork the repo to your account.  
   Go to the forked repo and clone it :busts_in_silhouette: to your local machine:

```sh
git clone https://github.com/Your_Username/QuickDoc.git
```

This will make a copy of the code to your local machine.

2. Now move to the `QuickDoc` directory.

```sh
cd QuickDoc
```

3. Now check the remote of your local code by:

```sh
git remote -v
```

The response should look like:

```sh
origin	https://github.com/Your_Username/QuickDoc.git (fetch)
origin	https://github.com/Your_Username/QuickDoc.git (push)
```

To add upstream to remote, run:

```sh
git remote add upstream https://github.com/Piyush-372002/QuickDoc
```

Again run `git remote -v`, the response should look like:

```sh
origin	https://github.com/Your_Username/QuickDoc.git (fetch)
origin	https://github.com/Your_Username/QuickDoc.git (push)
upstream	https://github.com/Piyush-372002/QuickDoc (fetch)
upstream	https://github.com/Piyush-372002/QuickDoc (push)
```

4. Once the remote is set, install all the necessary dependencies by the following command:

```sh
npm install
```
### Run locally

Run the below command to start the server:

```sh
npm run dev
```
Go to: [http://localhost:4000](http://localhost:4000)


