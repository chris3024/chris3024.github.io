<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

# CS-499 | Professional ePortfolio (Work In Progress)

### Introduction and Professional Self-Assessment

<hr style="width:100%; height:3px;">

### Portfolio Summary



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
<img src="screenshots/Screenshot 2025-05-18 125114.png"/>

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
<img src="screenshots/Screenshot 2025-05-30 110438.png"/>

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
<img src="screenshots/Screenshot 2025-06-10 115800.png"/>

<div class="button-group" style="text-align:center;">
  <a href="narratives/Sharp_Christopher_EnhancementThree_Databases.pdf" class="fancy-button" target="_blank" rel="noopener noreferrer">Full Narrative</a>
  <a href="https://github.com/chris3024/IT-145-Pet-Rescue" class="fancy-button" target="_blank" rel="noopener noreferrer">Original Artifact</a>
  <a href="https://github.com/chris3024/CS_499_Enhancement_3" class="fancy-button" target="_blank" rel="noopener noreferrer">Enhanced Artifact</a>
</div>
