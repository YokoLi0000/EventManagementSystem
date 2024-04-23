# EventManagementSystem

<< Description >>

The Event Management System aims to organize school events and provides a platform for students to register and participate in school activities in a much convenient way. It allows students to engage in different events, and enjoys meaningful and fruitful university life.

<< Execution >>
1. Download EventManagementSystem.bat and EventManagementSystem.jar
2. Put the two files in the same directory
3. Double click the EventManagementSystem.bat to run the program

<< User Guideline >>

Here are the commands for using the system:

-------------------------------Create-------------------------------

Create a student:
create student [studentID] [major] [first name] [last name] [sex] [age]
* studentID should be in the format of s12345678

Create an event for individual participation:
create event [event name] [eventID] [capacity] [date] [major]
* eventID should be in the format of e12345678

Create an event for group participation:
create event [event name] [eventID] [capacity] [date] [major] [group capacity] [minimum number of people in a group] [maximum number of people in a group]
* eventID should be in the format of e12345678

Create a group:
create group [groupID] [maximum number of people in a group]
* groupID should be in the format of g12345678

-------------------------------Delete-------------------------------

Delete a student:
delete student [studentID]
* studentID should be in the format of s12345678

Delete an event:
delete event [eventID]
* eventID should be in the format of e12345678

Delete a group:
delete group [groupID]
* groupID should be in the format of g12345678

--------------------------------Join--------------------------------

Student join an event:
studentJoin event [studentID] [eventID]
* studentID should be in the format of s12345678
* eventID should be in the format of e12345678

Student join a group:
studentJoin group [studentID] [groupID]
* studentID should be in the format of s12345678
* groupID should be in the format of g12345678

Group join an event:
groupJoin event [groupID] [eventID]
* groupID should be in the format of g12345678
* eventID should be in the format of e12345678

--------------------------------Quit--------------------------------

Student quit an event:
studentQuit [studentID] [eventID]
* studentID should be in the format of s12345678
* eventID should be in the format of e12345678

Student quit a group:
studentQuit [studentID] [groupID]
* studentID should be in the format of s12345678
* groupID should be in the format of g12345678

Group quit an event:
groupQuit [groupID] [eventID]
* groupID should be in the format of g12345678
* eventID should be in the format of e12345678

--------------------------------List--------------------------------

List all students:
list student

List all events:
list event

List all groups:
list group

List all events of a student joined:
list studentJoinedEvent [studentID] all
* studentID should be in the format of s12345678

List pending events of a student joined:
list studentJoinedEvent [studentID] pending
* studentID should be in the format of s12345678

List ended events of a student joined:
list studentJoinedEvent [studentID] end
* studentID should be in the format of s12345678

List all groups of a student joined:
list studentJoinedGroup [studentID]
* studentID should be in the format of s12345678

-------------------------------Search-------------------------------

Search an event by eventID:
search event id [eventID]
* eventID should be in the format of e12345678

Search events by major:
search event major [major]

Search a group by groupID:
search group [groupID]
* groupID should be in the format of g12345678

Search a student by studentID:
search student [studentID]
* studentID should be in the format of s12345678

------------------------------Recommend-----------------------------

Recommend events:
recommend [studentID]
* studentID should be in the format of s12345678

--------------------------------Help--------------------------------

List all commands:
help
