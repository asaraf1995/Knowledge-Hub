## Table of Contents
1. [Database](#database)
1. [Author(s)](#author)
1. [Database description](#description)
 
# Database
knowledge_hub

# Author(s)

Aastha Saraf
Akshay Narula

# Database description

An author and the reviewer creates and adds content which is consumed by the user. The activities of the users are then tracked to mark the progress and completion of the content.

author(id, name, content_id)

reviewer(id, name, content_id)

content(id, name, description, isActive)

content_pages(content_id, id, type, path)

user(id, name)

user_activity(user_id, content_id, page_id, viewed_on)




Base project Demo. Using three entities, spring microservises, html/jquery.

# Rubric Requirements 
1. *The SQL query implement the complete database including 
 other constraints (different to FK and PK)*: \
 Apart from FK and PK **'NOT NULL' and 'DEFAULT'** constraints added
 
1. *The forms have validations or preview of the data for detele or update*: \
The name should have only alphabets 
and email should contain '@','.' for ex: xyz@xyz.xyz \
**(name and email are mandatory fields with 'NOT NULL' constraint)** \
**Implemented for all the CRUD entities**

1. *Implement three simple queries*: 
   * Get names of all the contents with their Authors and Reviewers
   * Get the name of the Course and the Reviewer with a pending course (Not approved by the Reviewer to be available to the Users is active=0)
   * Get the content name where the Author and the Reviewer have the same email id

1. *Implement five complex queries*:
   * Get the Author name with most courses authored
   * Get the User's name who has completed one and only one course
   * Get the User's name who has completed all the courses
   * Get the User's name who hasn't been active since a week
   * Get all the User's ranked based on their overall content progress
 
