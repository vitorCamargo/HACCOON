# HACCOON - Haken Central Control Online

HACCOON is a project developed by the members of the Haken who are attending the discipline of Integrator Project and Software Engineering at Universidade technological Federal do Paraná, campus of Campo Mourão (UTFPR-CM).

## Summary
* [System Overview](#system-overview)
  * [Team Management](#team-management)
  * [File Management](#file-management)
  * [Customer Management](#customer-management)
  * [Project Management](#project-management)
  * [Goals Management](#goals-management)
  * [Calendar System](#calendar-system)
  * [Chat System](#chat-system)
  * [Gamification Subsystem](#gamification-subsystem)

* [Used Softwares and Technologies](#used-softwares-and-technologies)

To see more about the Visual Identity and Design Concepts used in this project, [click here](/DESIGN.md).

## System Overview
This system aims to [manage the team](#team-management), [file management](#file-management), [customer management](#customer-management), [project management](#project-management), [goals management](#goals-management), a [calendar system](#calendar-system), an [integrated chat system](#chat-system) and a [gamification subsystem](#gamification-subsystem).

### Team Management
Team management will be done with respect to the hierarchy rule: When a person enters the company, it is considered a **trainee**, after a training in the company it becomes a **member** and if possible can become a **director**.

Directors can add (create new accounts) for trainees and new customers to have access to the system, update the positions of members for directors, and delete users from the system.
They can also add warnings to members or add points to the [gamification subsystem](#gamification-subsystem), viewing project files, contracts, planning pokers and other [files](#file-management). In addition to creating new projects and attaching members or trainees that will make it.

The great difference between members and trainees is that projects attached to members also have an attachment to a customer, while a trainee can only carry out internal projects of the company.
For both members and trainees it is only possible that they view their own projects (past and present) and the project status, but in another projects it is just possible to view basic informations about it.

### File Management
Currently all company files are stored in the company's Google Drive account. It is entirely necessary to use an API to access the files, be able to add new ones, remove them, edit them (even externally) and view them as well, or perhaps, create a system that add files in a file server and link to our database with a organization arround the file (like directories).

### Customer Management
It is necessary for the company to have a contact list and the profile of each customer who contacts the company. For this to happen, the directors will be able to add new customers to the system, allowing them to access the platform, however, it is known that not every client will use the platform as a form of communication, so it should appear in your profile a link with your Whatsapp. Remembering that it should be possible for the client to send messages to the Project Director and also view the status of your project.

### Project Management
Directors can create a project, assign a status (canceled, in progress, finished, etc...) and embed the project with GitHub (it will be interesting to see the progress of issues or other information from GitHub itself using an API), you can also Add the developer and client members of the project, as well as information such as important links, planning poker files, and other projects (when a project is renewed in the enterprise).

### Goals Management
Directors can add goals for the year, the idea behind this management is for the system use all informations collected like, projects done, how much each project cost it. And create a metric about a specific goal.

### Calendar System
In this area of the system, the directors can create new events in calendar, add photos in a determinate event, link with the members whose went in it.

### Chat System
The chat works in a simple way, any employee can send messages to any employee of the company (not counting the person's hierarchy), you can also create group with people. The only rule imposed is that essentially only the directors can contact customers and vice versa.
For the chat, will be used as a form of communication: text, emojis, gifs and images (stickers), any other way will be an additional to the system (for example: audio and file submission).

### Gamification Subsystem
The gamification subsystem is still a new subject in the company, for a first step it is necessary to construct a table with all the tasks that generate points and their score. The directors are responsible for managing the table and distributing points to the members and trainees. In the profile of the members/trainees should appear a history of scores, showing the task, the earned points and the day in won.

It would be interesting for the directors to be shown the points with graphs or forms of representation of data that help in the visualization and choice of the best members, *although this is considered an additional functionality of the system*.

## Used Softwares and Technologies
As the project is being produced by Haken members for Haken members, will be used programming languages, tools and frameworks already used by the company, the following is a table of the software and its use in the project:

|  Software  |                                            Used For                                            |
|:----------:|:----------------------------------------------------------------------------------------------:|
|   ReactJS  | JavaScript library for building user interfaces.                                               |
| AntDesign  | UI design language and React-based implementation with a set of high-quality React components. |
|   NodeJS   | Focused on migrating client-side Javascript to servers.                                        |
|   Express  | NodeJS web application framework that provides a set of features for web applications          |
|   MongoDB  | MongoDB is a document-oriented database program, classified as a NoSQL database program.       |
|   Heroku   | Cloud platform as a service supporting javascript language.                                    |
|    mLab    | mLab is a fully managed cloud database service that hosts MongoDB databases.                   |
| Cloudinary | Provides a cloud-based image and video management solution (files too).                        |
