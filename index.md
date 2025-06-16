<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

# CS-499 | Professional ePortfolio 

### Introduction and Professional Self-Assessment

My name is Christopher, and I began pursuing a Bachelor’s degree in Computer Science with a concentration in Information Security in October 2020. Balancing a full-time job, family life, and coursework has been one of the biggest challenges I’ve faced, but also one of the most rewarding. It taught me how to manage my time effectively, stay focused, and push through when things got tough.

Throughout the program, I built a strong foundation in software development, databases, algorithms, and secure coding practices. I’ve worked on a variety of projects that pushed me to think critically, write maintainable code, and apply what I’ve learned to real-world scenarios. Over time, I’ve grown more confident in my ability to design and build systems that are both functional and secure. While most of the program involved independent work, I made improvements based on instructor feedback and carried those revisions through multiple enhancements. This helped me develop habits that support collaboration, such as clear documentation, version control, and focusing on usability for different users.

Developing my ePortfolio gave me the chance to bring all of these skills together. I enhanced previous coursework to reflect industry standards, added functionality, improved usability, and focused on security best practices. I also recorded a code review video to walk through the enhancements, explain the original code base and issues, and discuss the plan to improve upon them.

In addition to coding, I completed courses that covered networking, systems administration, and cybersecurity fundamentals. These included working with virtual machines, firewall configuration, vulnerability scanning, and applying security frameworks to systems and applications. Some classes used hands-on labs and tools like TestOut Network+, which gave me experience with real-world IT environments and troubleshooting scenarios. Other courses covered access control, encryption, and software hardening—skills I applied directly in my final enhancements.

I’ve also gained experience with data structures like AVL trees and hashmaps, implemented secure CRUD operations using MongoDB, and followed secure coding practices like hashing passwords and enforcing login rules. These technical skills, combined with a solid foundation in problem solving and system design, have prepared me for a role in IT or software development.

This program helped me grow not just as a developer but as a professional. I’m confident in my ability to contribute to real-world projects and continue learning as I move forward in the field. This experience has also helped confirm my interest in working in IT, especially in areas like technical support, secure application development, or system administration.

<hr style="width:100%; height:3px;">

### Portfolio Summary

The first enhancement in my portfolio falls under the category of **Software Design and Engineering**. This enhancement involved transforming an early Java-based console application, created for a fictional animal rescue organization called Grazioso Salvare, into a modern Python application with a graphical user interface using Tkinter. The original version featured a basic menu-driven system but lacked usability and persistent data storage. In the refactored version, I addressed these issues by building an intuitive GUI and implementing JSON file-based data persistence. The modular structure of the application and the use of GitHub Actions for static analysis, testing, and code quality enforcement allowed for a more professional and maintainable codebase. This enhancement demonstrates my skills in object-oriented programming, cross-language development, GUI design, file handling, and the integration of continuous integration and deployment tools. It also showcases my ability to produce clear documentation tailored to technical audiences.

The second enhancement addresses the category of **Algorithms and Data Structures**. The original artifact, a C++ application created for CS 300, was designed to assist academic advisors by allowing them to view and search a course catalog imported from a CSV file. The initial implementation used vectors and quicksort for sorting, resulting in moderate efficiency. To improve performance and scalability, I replaced the data structure with a self-balancing AVL tree, achieving faster search and insert operations. I also modernized the C++ codebase by incorporating smart pointers to enhance memory safety and reduce the risk of leaks, while also adding robust error handling, null checks, and input sanitization. This enhancement reflects a deeper understanding of algorithmic principles and time complexity analysis, and it demonstrates secure and reliable programming practices. Tools such as GitHub Actions, MSBuild, and CodeQL were used to automate building, testing, and static code analysis.

The third and final enhancement pertains to the category of **Databases**. This work builds directly upon the first enhancement by replacing the JSON file storage with a MongoDB NoSQL backend. This transition enabled more scalable data handling, efficient queries, and improved application performance. I developed a dedicated AnimalDatabase class to separate database operations from GUI logic, and I integrated user authentication and role-based access control into the application. Passwords are securely hashed, and new users are prompted to change their passwords upon first login. The GUI dynamically updates based on the user's role, ensuring both usability and security. Document validation rules were added to the MongoDB collections to ensure data integrity. This enhancement highlights my ability to work with production-ready database systems, apply security best practices, and design scalable, modular software systems. It also reinforces my experience with continuous integration and deployment practices through automated testing, linting, and scanning via GitHub Actions.

<hr style="width:100%; height:3px;">

### Code Review Video

In this code review video, I describe the original artifacts and their origins and how the code functions. I also touch upon some of the faults that I found in the code. Finally, I break down the planned
enhancements for the code and how it aligns with the course outcomes.
<div style="position: relative;"> 
  <iframe width="560" height="315" 
    src="https://www.youtube.com/embed/wVK2klug9gw?si=hs3apkGi6iQNJYci" 
    title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; 
    picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
  </iframe>
</div>
<br>

<hr style="width:100%; height:3px;">

### Software Design and Engineering

***Description:*** The original artifact for this enhancement comes from a project we completed in my IT-145: Foundation in Application Development course. This software is a console application written in the Java programming language for the client Grazioso Salvare and their rescue animal operations. When started, the application displays a menu system in a console environment and allows the user to select different options, ranging from the intake of a new animal, displaying all the registered animals, and updating the status of the animals.

***Enhancement:*** To enhance this program, we have expanded the application by introducing a graphical user interface (GUI) built using the tkinter framework to improve usability. Additionally, we enhanced the software by incorporating file input/output capabilities to save data in JSON format, ensuring persistence across application runs. 

#### Main GUI Window
<img src="screenshots/Screenshot 2025-05-18 125114.png" style="max-width: 100%; height: auto"/>

<div class="button-group" style="text-align:center;">
  <a href="narratives/Sharp_Christopher_EnhancementOne_SoftwareDesignandEngineering.pdf" class="fancy-button" target="_blank" rel="noopener noreferrer">Full Narrative</a>
  <a href="https://github.com/chris3024/IT-145-Pet-Rescue" class="fancy-button" target="_blank" rel="noopener noreferrer">Original Artifact</a>
  <a href="https://github.com/chris3024/CS_499_Enhancement_1" class="fancy-button" target="_blank" rel="noopener noreferrer">Enhanced Artifact</a>
</div>


<hr style="width:100%; height:3px;">

### Algorithms and Data Structures
***Description:*** The original artifact for this enhancement comes from the coursework that was completed in CS-300: Data Structures and Algorithms, Analysis and Design. This console-based C++ program was created to assist academic advisors at the fictional university, ABCU. This application imports the data from a CSV file and inserts it into a vector data structure for partitioning and sorting. Then, from a menu system, users can list the courses in alphabetical order or search for a specific course, returning its data, which includes the course number, name, and any prerequisites. 

***Enhancement:*** For the enhancement in this category, I decided to replace the vector data structure, which is neither the most efficient nor scalable, with the use of a self-balancing AVL tree. By replacing it with a self-balancing AVL tree, we are allowing for more scalability of the software, but also allowing for quicker insertions and lookups. Also, the code was modernized with the introduction of unique pointers, which allow for automated memory management, and the implementation of null checks, input sanitization, and structured exception handling increased the security of the software. 


### Insertion Method for AVL tree
<img src="screenshots/Screenshot 2025-05-30 110438.png" style="max-width: 100%; height: auto"/>

<div class="button-group" style="text-align:center;">
  <a href="narratives/Sharp_Christopher_EnhancementTwo_AlgorithmsAndDataStructures.pdf" class="fancy-button" target="_blank" rel="noopener noreferrer">Full Narrative</a>
  <a href="https://github.com/chris3024/CS-300-DSA-Advisor-Program" class="fancy-button" target="_blank" rel="noopener noreferrer">Original Artifact</a>
  <a href="https://github.com/chris3024/CS_499_Enhancement_2" class="fancy-button" target="_blank" rel="noopener noreferrer">Enhanced Artifact</a>
</div>

<hr style="width:100%; height:3px;">

### Databases
***Description:*** The original artifact for this enhancement comes from a project we completed in my IT-145: Foundation in Application Development course. This code was refined for enhancement one, software design and engineering, with the implementation of a Graphical User Interface (GUI) and data persistence with the use of JSON files, while keeping all of the same functionality of the original code base. 

***Enhancement:*** For the enhancement in this category, I took the Grazioso Salvare Animal Rescue application and replaced the implementation of file I/O with the use of MongoDB. For this, I created the CRUD schema that performed the operations of creating, reading, updating, and deleting the data from the database. In addition to the use of a database for data persistence, the security of the application was also enhanced. For this, role-based access control (RBAC) was implemented with the use of hashed and salted passwords using the bcrypt library.

#### Main Application Window (Login Window)
<img src="screenshots/Screenshot 2025-06-10 115800.png" style="max-width: 100%; height: auto"/>

<div class="button-group" style="text-align:center;">
  <a href="narratives/Sharp_Christopher_EnhancementThree_Databases.pdf" class="fancy-button" target="_blank" rel="noopener noreferrer">Full Narrative</a>
  <a href="https://github.com/chris3024/IT-145-Pet-Rescue" class="fancy-button" target="_blank" rel="noopener noreferrer">Original Artifact</a>
  <a href="https://github.com/chris3024/CS_499_Enhancement_3" class="fancy-button" target="_blank" rel="noopener noreferrer">Enhanced Artifact</a>
</div>
