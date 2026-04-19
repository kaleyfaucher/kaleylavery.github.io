# Enhancement 3 – Databases

[Home](index.md) | [Artifacts Overview](artifacts.md) | [Enhancement 1](enhancement1.md) | [Enhancement 2](enhancement2.md)

## Artifact Files
- Original Artifact (to be added)
- Enhanced Artifact (to be added)
- Narrative Document (to be added)

## Artifact Description
The artifact selected for this enhancement is the Travlr Getaways full-stack web application, originally developed in CS 465. This application uses a MongoDB database with Mongoose as the object data modeling (ODM) library to manage trip-related data. The application allows users to view, create, update, and delete travel packages through a RESTful API. The database layer plays a critical role in storing and retrieving structured trip data, which is then consumed by both the public-facing site and the administrative interface.

## Justification for Inclusion
This artifact was selected because it demonstrates my ability to design and implement a full-stack application with a functional database layer. It highlights my experience working with MongoDB and Mongoose, as well as my ability to integrate database operations with an API-driven backend. The original implementation included a basic schema structure, but it lacked more advanced validation and data integrity controls that are expected in production-level applications.

Enhancing this artifact allowed me to demonstrate my ability to improve database design by implementing stronger validation rules, enforcing data consistency, and aligning the schema with industry best practices. These improvements directly showcase my skills in database management and backend development.

## Enhancement Description
The primary enhancement made to the database component was the improvement of the Mongoose schema for the Trip model. While the original schema included basic validation such as required fields, this enhancement introduced more advanced data validation and structural improvements.

Specifically, I updated the `start` field from a string data type to a Date object. This change allows for more accurate handling of date-based data and enables better querying and sorting capabilities within the application. I also added a minimum length validation to the `description` field to ensure that meaningful and complete information is stored in the database. Additionally, I implemented automatic timestamp tracking using Mongoose’s built-in `timestamps` option, which records when each document is created and last updated.

These enhancements improve the overall integrity and usability of the database by ensuring that data is stored in a consistent and reliable format. They also align the application more closely with real-world database design practices.

## Course Outcomes Alignment
This enhancement supports multiple course outcomes from the Computer Science program.

First, it demonstrates my ability to design and evaluate computing solutions by improving the structure and validation of the database schema. By selecting appropriate data types and validation rules, I ensured that the application handles data more effectively and efficiently.

Second, it reflects my ability to use well-founded and innovative techniques, skills, and tools in computing practices. The use of Mongoose validation, schema configuration, and timestamp tracking shows my understanding of industry-standard tools and practices for database management.

Third, this enhancement highlights my development of a security mindset. By enforcing validation rules and preventing invalid data from being stored, I reduced potential vulnerabilities related to data integrity and input handling. Ensuring that only properly formatted data is accepted into the system is a key aspect of secure application design.

Finally, this work demonstrates my ability to communicate technical improvements clearly, as shown through this narrative and the explanation of the enhancement process. Being able to articulate the purpose and impact of technical changes is an essential skill in collaborative development environments.

## Reflection on the Enhancement Process
Throughout the enhancement process, I gained a deeper understanding of how important data validation and schema design are in maintaining the quality and reliability of an application. Initially, my focus was primarily on functionality, ensuring that the application could perform CRUD operations. However, this enhancement required me to think more critically about how data is structured and validated at the database level.

One of the key challenges I encountered was ensuring that changes to the schema did not break existing functionality within the application. Changing the `start` field to a Date type required careful consideration of how that data is handled throughout the system. This reinforced the importance of understanding how different components of an application interact with each other.

Additionally, this process helped me recognize the importance of anticipating potential issues, such as invalid or incomplete data being entered into the system. By implementing stronger validation rules, I was able to reduce the likelihood of these issues and improve the overall robustness of the application.
