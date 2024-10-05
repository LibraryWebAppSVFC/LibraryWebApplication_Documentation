# Library Web Application

## INTRODUCTION

In today's digital age, fostering a love for reading and learning from an early age is more crucial than ever. 
Recognizing the need for a platform that caters to the unique needs of young learners, their parents, and educators, 
we are excited to introduce our project: the Library Web App. The Library Web App is designed to be a comprehensive, 
user-friendly online platform that transforms the way educational resources are accessed and managed. Tailored 
specifically for young children, this application aims to provide a seamless and engaging experience for its young 
users while offering robust tools for parents and teachers. The website features an intuitive layout and an appealing 
color scheme, with carefully chosen fonts to ensure ease of navigation and to create an inviting atmosphere for its 
diverse audience. Our goal with the Library Web App is to create a digital environment where learning is both enjoyable 
and accessible. By prioritizing simplicity and visual appeal, we aim to support young readers in their educational 
journey, empower parents to actively participate in their children's learning, and assist educators in managing and 
delivering valuable resources effectively. Through this project, we aspire to build a bridge between education and 
technology, making it easier for families and schools to engage with and benefit from the wealth of knowledge available 
in today’s digital world.


## Project Features and Characteristics
The Library Web App aims to create an easy-to-use platform that helps young children improve their reading and writing skills. It also offers support for parents and teachers. Here are the main features and qualities of the web app.
   #### Admin Book Management:
##### Book Storage: Admins can easily upload, organize, and manage a diverse collection of books, including poems, tales, and educational materials.
##### Categorization and Tagging: Books can be categorized and tagged for efficient searching and organization, allowing for easy retrieval based on genre or educational focus.
##### Metadata Management: Admins can add and edit detailed metadata for each book, including title, author, publication year, and summary, to provide users with comprehensive information.
   #### User-Friendly Interface:
##### Intuitive Design: The web app features a straightforward, visually appealing layout designed to be easily navigable by young children, parents, and educators.
##### Engaging Visuals: A vibrant color scheme and child-friendly fonts are used to create an inviting and engaging atmosphere that encourages exploration and interaction.
   #### Access and Navigation:
##### Easy Search and Filter Options: Users can quickly find books using search functions and filters based on categories, age groups, and reading levels.
##### Personalized Recommendations: The app offers book recommendations based on user preferences and previous interactions, helping users discover new and relevant resources.
   #### User Profiles and Progress Tracking:
##### Custom User Accounts: Children, parents, and educators can create personalized accounts to track reading progress and access tailored recommendations.
##### Progress Reports: Users can view and track their reading progress and achievements, providing insights into learning milestones and areas for improvement.


## Project Scope

1. Design and implement a user-friendly web application optimized for both desktop and mobile, featuring a child-friendly interface with engaging visuals.
2. Develop an admin dashboard for efficient management of a diverse collection of books and educational materials, including poems, stories, and interactive resources.
3. Create personalized user accounts with tracking of reading progress and tailored recommendations to enhance the learning experience.
4. Implement advanced search and filter options to help users easily find books and resources through book categories.




## Work breakdown Structure

![image](https://raw.githubusercontent.com/TheLastWeaboo/LibraryWebApplication_Documentation/refs/heads/main/work%20breakdown%20structure1.png)

## Functional Requirements

#### 1. User Registration and Authentication
###### FR1.1: The system shall allow users to register with a unique username, email, and password.
###### FR1.2: The system shall allow users to log in using their email and password.
###### FR1.3: The system shall support different user roles (e.g., child, parent, admin).
#### 2. User Profile Management
###### FR2.1: The system shall allow users to view and edit their profile information, including username, email, and date of birth.
###### FR2.2: The system shall allow users to view their reading history and progress.
#### 3. Book Management
###### FR3.1: The system shall allow administrators to add, edit, and delete books in the library.
###### FR3.2: The system shall allow administrators to upload book cover images and other related metadata.
###### FR3.3: The system shall allow users to browse and search for books by title, author, genre, and category.
FR3.4: The system shall display detailed information about each book, including title, author, genre, summary, and cover image.
#### 4. Reading Experience
###### FR4.1: The system shall allow users to read books online within the application.
###### FR4.2: The system shall allow users to navigate between chapters of a book.
###### FR4.3: The system shall save the user's reading progress and allow them to resume reading from where they left off.
###### FR4.4: The system shall support bookmarking specific pages or chapters.
#### 5. Reading Progress and History
###### FR5.1: The system shall track the user's reading progress for each book.
###### FR5.2: The system shall allow users to view their reading history and continue reading previously started books.
###### FR5.3: The system shall allow users to view a summary of their reading progress, including books completed and time spent reading.
#### 6. Book Categories
###### FR6.1: The system shall allow administrators to create, edit, and delete book categories.
###### FR6.2: The system shall allow users to browse books by category.
###### FR6.3: The system shall allow users to filter books by multiple categories.
#### 7. Administrative Functions
###### FR7.1: The system shall allow administrators to manage user accounts, including adding, editing, and deleting users.
###### FR7.2: The system shall allow administrators to generate reports on user activity, book popularity, and overall system usage.
###### FR7.3: The system shall provide tools for monitoring and moderating user-generated content, such as reviews.
#### 8. Security
###### FR8.1: The system shall enforce strong password policies for user accounts.
###### FR8.2: The system shall protect user data with encryption and secure authentication methods.
                                                                                                                                |

### use case
![image](https://raw.githubusercontent.com/TheLastWeaboo/LibraryWebApplication_Documentation/refs/heads/main/usecase.png)

## Database Architecture

### Data Dictionary
### Database Architecture

#### Table 1: USERS

| FIELD NAME   | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE             |
|--------------|--------------------------------------|-----------|--------|--------------------|
| USER_ID      | Unique Identification of User        | String    | 255    | UID123456789       |
| USERNAME     | User's login name                    | String    | 255    | booklover89        |
| EMAIL        | User's email address                 | String    | 255    | user@example.com   |
| PASSWORD_HASH| Encrypted password                   | String    | 255    | [encrypted string] |
| ROLE         | Role of the user (child, parent, admin) | String | 50     | child              |
| DATE_OF_BIRTH| User's date of birth                 | Date      |        | 2010-05-15         |
| CREATED_AT   | Timestamp of user creation           | Date      |        | 2024-08-23 14:00:00|
| UPDATED_AT   | Timestamp of last update             | Date      |        | 2024-08-23 14:00:00|

#### Table 2: BOOKS

| FIELD NAME      | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE                                                           |
|-----------------|--------------------------------------|-----------|--------|------------------------------------------------------------------|
| BOOK_ID         | Unique Identification of Book        | String    | 255    | BID987654321                                                     |
| TITLE           | Title of the book                    | String    | 255    | The Adventures of Tom Sawyer                                     |
| AUTHOR          | Author of the book                   | String    | 255    | Mark Twain                                                       |
| GENRE           | Genre of the book                    | String    | 255    | Fiction                                                          |
| PUBLICATION_DATE| Date the book was published          | Date      |        | 1876-06-01                                                       |
| ISBN            | International Standard Book Number   | String    | 13     | 9781234567897                                                    |
| LANGUAGE        | Language of the book                 | String    | 100    | English                                                          |
| SUMMARY         | Brief summary of the book            | Text      |        | A novel about a young boy growing up along the Mississippi River... |
| COVER_IMAGE_URL | URL of the book's cover image        | String    | 255    | https://example.com/tomsawyer.jpg                                |
| CREATED_AT      | Timestamp of book creation           | Date      |        | 2024-08-23 14:00:00                                              |
| UPDATED_AT      | Timestamp of last update             | Date      |        | 2024-08-23 14:00:00                                              |


#### Table 3: READING_PROGRESS

| FIELD NAME          | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE             |
|---------------------|--------------------------------------|-----------|--------|--------------------|
| PROGRESS_ID         | Unique Identification of Progress    | String    | 255    | RP123456789        |
| USER_ID             | Foreign Key to User ID               | String    | 255    | UID123456789       |
| BOOK_ID             | Foreign Key to Book ID               | String    | 255    | BID987654321       |
| CHAPTER_ID          | Foreign Key to Chapter ID            | String    | 255    | CH123456789        |
| PROGRESS_PERCENTAGE | Percentage of book read              | Decimal   |        | 75.00              |
| LAST_READ_AT        | Timestamp of last read               | Date      |        | 2024-08-23 15:30:00|

#### Table 4: CATEGORIES

| FIELD NAME   | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE             |
|--------------|--------------------------------------|-----------|--------|--------------------|
| CATEGORY_ID  | Unique Identification of Category    | String    | 255    | CAT123456789       |
| NAME         | Name of the category                 | String    | 255    | Adventure          |
| DESCRIPTION  | Description of the category          | Text      |        | Books full of thrilling adventures |
| CREATED_AT   | Timestamp of category creation       | Date      |        | 2024-08-23 13:00:00|
| UPDATED_AT   | Timestamp of last update             | Date      |        | 2024-08-23 13:00:00|

#### Table 5: BOOK_CATEGORIES

| FIELD NAME        | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE             |
|-------------------|--------------------------------------|-----------|--------|--------------------|
| BOOK_CATEGORY_ID  | Unique Identification of Relation    | String    | 255    | BC123456789        |
| BOOK_ID           | Foreign Key to Book ID               | String    | 255    | BID987654321       |
| CATEGORY_ID       | Foreign Key to Category ID           | String    | 255    | CAT123456789       |




## ERD

For Best View
(https://lucid.app/lucidchart/99c7cf6d-20eb-4671-8235-4d7d5200c72e/edit?beaconFlowId=585138D6FE0691C7&invitationId=inv_58d5808b-a6a7-4fa3-8c5a-46956bb25276&page=0_0)


![image](https://raw.githubusercontent.com/LibraryWebAppSVFC/LibraryWebApplication_Documentation/refs/heads/main/erd.png)


## Non Functional Requirements

### Product Requirement (PLEASE SKIP THIS)

### Organizational Requirement (PLEASE SKIP THIS)


### External Requirements  (PLEASE SKIP THIS)


## System Testing and Evaluation   (PLEASE SKIP THIS)

### Functional Testing Procedure   (PLEASE SKIP THIS)

### Functional Testing Summary

### Evaluation Procedure

### Recommendation






### Wireframe (PLEASE SKIP THIS)



### High Fidelity (PLEASE SKIP THIS)



### System Screenshot (PLEASE SKIP THIS)
