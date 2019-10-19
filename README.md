# Unit 05 Third-Party APIs Homework: Day Planner

Create a simple calendar application that allows the user to save events for each hour of the day. This app will run in the browser and feature dynamically updated HTML and CSS powered by jQuery.

The app should display standard business hours (9 a.m. to 5 p.m.). Each time slot should represent one hour and contain the following:

* The time

* A field to hold user input

* A save button

Clicking on the save button will store the time and user input in `localStorage`.

Near the top of the calendar, the application should display the current day. Additionally, each hour should be color coded to reflect whether the time slot is in the past, the present, or the future. This will change depending on the time of day.

You'll need to use the [Moment.js](https://momentjs.com/) library to work with date and time. Be sure to read the documentation carefully and concentrate on using Moment.js in the browser.

![day planner demo](./Assets/05-Third-Party-APIs-homework-demo.gif)

## User Story

AS AN employee with a busy schedule

I WANT to add important events to a daily planner

SO THAT I can manage my time effectively 

## Business Context

Poor time management can result in missed meetings and deadlines or create the appearance of unprofessionalism. A daily planner allows employees to see their day at a glance, schedule time effectively, and improve productivity. 

## Minimum Requirements

* Functional, deployed application.

* GitHub repository with a unique name and a README describing project.

* The application displays timeblocks for standard business hours (9 a.m. to 5 p.m.).

* Each timeblock contains an input field and save button.

* Clicking a timeblock's "Save" button stores the input text in local storage, allowing the text to persist when the application is refreshed.

* The current day is displayed at the top of the calendar.

* Each timeblock is color coded to indicate whether it is in a past, present, or future hour.

```
GIVEN that an employee adds events to a specific hour in a calendar

WHEN the employee clicks the save button

THEN events are saved in the timeblock for that hour
```
- - -
Matt Atchley
Initial Comments

when loaded it does not have any hours blocked
main title screen is not fixed
no color for times
has a similar look to the todo list and requirements
must be in jquery
the html has no code for the time blocks
there is bootstrap in the html that will allow for styling ease

Step 1
Pseudocode
From observing the gif I will need to use similar functions to the todo list activity and dynamic creation of content from the quiz homework.

Q: can you put jquery on a seperate file?

step 1
for the main content of the page there needs to be some sort of For Loop that creates the time blocks from an array of 9am-5pm
-this may be styled with boot strap
done (x) 10-15 2:25

step 2 
allow for the user to save items that are within the time blocks
half way? 10-15 4pm
found a way to fix it by making the renderPlans append to their own seperate div

Step3
Integrate time into page, moment.js?
Logic is there and can be styled by the CSS

step 4 Change local storage to set and get only no need for the array