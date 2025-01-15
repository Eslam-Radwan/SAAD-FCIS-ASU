### System Analysis and Design  
#### Finalizing Design Specifications  
**Prof. Rania Elgohary**  
rania.elgohary@cis.asu.edu.eg  
**Dr. Yasmine Afify**  
yasmine.afify@cis.asu.edu.eg  

---

### Chapter 13: Finalizing Design Specifications  
[FIGURE] The systems development life cycle with design phase highlighted  

- **Planning**  
- **Maintenance**  
- **Analysis**  
- **Implementation**  
- **Design**  
  - Databases  
  - Forms and Reports  
  - Dialogues and Interfaces  
  - Finalizing Design Specifications  
  - Distributed and Internet Systems  

---

### Good Specifications  
Good specifications should be stated:  
- Simply  
- Completely  
- Unambiguously  
- With attributes that make requirements more understandable  

---

### Deliverables and Outcomes  
- A set of physical design specifications for the entire system, with detailed specifications for each separate part of the system.  
  - Include functional descriptions for each part of the system.  
  - Include input received and output generated for each program and its component parts.  

---

### Specification Documents  
Contains:  
- Overall system description  
- Interface requirements  
- System features  
- Nonfunctional requirements  
- Supporting diagrams and models  

---

### Requirements Management (RM) Tools  
- Requirements management tools make it easier to keep documents up to date, add additional requirements, and link related requirements.  
- **10 Best Requirements Management Tools**:  
  - IBM Rational  
  - Accompa  
  - PREEB  
  - peats  
  - HelixALM  

---

### Benefits of Requirements Management Tools  
- Remove ambiguity  
- Ensure your implementation and deliverables are:  
  - Clear  
  - Realistic  
  - Agreed-upon  

---

### Designing Programs  
- Analysts should create a design of a maintainable system that is modular and flexible.  
- Analysts can design programs in a top-down modular approach.  

---

### Structure Chart  
- A high-level diagram, called a structure chart, is created to illustrate the organization and interaction of the different pieces of code within the program.  
- Program specifications are written to describe what needs to be included in each program module.  
- At the end of program design, the project team compiles the program design document.  

---

### Structure Chart (Cont.)  
- A hierarchical diagram that shows how an information system is organized.  
- Important program design technique that helps the analyst design the program.  
- It shows all components of code in a hierarchical format that implies:  
  - **Sequence** (order of invoking components)  
  - **Selection** (under what condition module is invoked)  
  - **Iteration** (how often component is repeated)  

---

### Structure Chart Symbols  
- **Data couple**: Diagrammatic representation of the data exchanges between two modules.  
- **Control couple (Flag)**: Diagrammatic representation of a message passed between two modules.  

---

### Linking DFDs to Structure Charts  
- Each process of a DFD tends to represent one module on the structure chart.  
- If leveled DFDs are used, then each DFD level tends to correspond to a different level of the structure chart hierarchy.  
- The process on the context-level DFD would correspond to the top module on the structure chart.  

---

### Steps in Building the Structure Chart  
1. Identify top-level modules and decompose them into lower levels.  
2. Add control connections (loops, conditional lines, etc.).  
3. Add couples (identify the information that has to pass among the modules, i.e., data couple and control couple).  
4. Review and revise again and again until complete.  

---

### Example: Academic System  
- An academic system needs a program that will print a listing of students along with their grade point averages (GPAs), both for the current semester and overall.  
- The program must:  
  1. Retrieve the student grade records.  
  2. Calculate the current and cumulative GPAs.  
  3. Print the grade list.  

---

### Structure Chart Example  
[FIGURE] Structure Chart for Student Grade Listing  

---

### Cohesion and Coupling  
- **Cohesion**: Refers to how well the lines of code within each module relate to each other.  
- **Coupling**: The measure of the independence of components. It defines the degree of dependency of each module of system development on the others.  

---

### Cohesion Types  
| Type               | Definition                                                                 | Example                                                                 |
|--------------------|---------------------------------------------------------------------------|-------------------------------------------------------------------------|
| **Functional**     | All elements of the module contribute to performing a single task.         | Calculate Current GPA                                                  |
| **Sequential**     | Output from one task is used by the next.                                  | Format and Validate Current GPA                                        |
| **Communicational**| Elements contribute to activities that use the same inputs or outputs.     | Calculate Current and Cumulative GPA                                   |
| **Procedural**     | Elements are performed in sequence but do not share data.                  | Print Grade Listing                                                    |
| **Temporal**       | Activities are related in time.                                            | Initialize Program Variables                                           |
| **Logical**        | List of activities; which one to perform is chosen outside of the module.  | Perform Customer Transaction                                           |
| **Coincidental**   | No apparent relationship.                                                  | Perform Activities                                                     |

---

### Advantages of High Cohesion  
- Improved readability and understandability.  
- Better error isolation.  
- Improved reliability.  

---

### Coupling Types  
| Type               | Definition                                                                 |
|--------------------|---------------------------------------------------------------------------|
| **Content Coupling**| When one component modifies another, making the modified component dependent. |
| **Common Coupling**| When data is accessible from a common data store.                         |
| **Control Coupling**| When one component passes parameters to control the activity of another.  |
| **Stamp Coupling** | When data structures are used to pass information between components.     |
| **Data Coupling**  | When only data is passed between components.                              |

---

### Advantages of Low Coupling  
- Improved maintainability.  
- Enhanced modularity.  
- Better scalability.  

---

### Fan-In and Fan-Out  
- **Fan-in**: Describes the number of control modules that communicate with a subordinate.  
- **Fan-out**: The number of subordinates associated with a single control.  

---

### Program Specification  
- Once the analyst has communicated the big picture of how the program should be put together, they must describe the individual modules in enough detail so that programmers can begin writing code.  
- **Program Specification Components**:  
  - Program information  
  - Events  
  - Inputs and outputs  
  - Pseudocode  

---

### UI Design  
- Many users access web material on handheld devices than on desktops.  
- **Adaptive Design**: Craft several versions of one design with fixed dimensions.  
- **Responsive Design**: Work on a single, flexible design that adjusts to various screen sizes.  

---

### Responsive Design Core Principles  
- Fluid Grid System  
- Fluid Image Use  
- Media Queries  

---

### Fluid Grid System  
- Elements occupy the same percentage of space regardless of screen size.  
- Use CSS grid systems and generators for the design’s base.  

---

### Fluid Image Use  
- Images default to the same size and configuration across devices.  
- Apply CSS command: `img {max-width: 100%;}` to ensure images shrink for smaller screens.  

---

### Media Queries  
- Filters used to detect the browsing device's dimensions and adjust the design accordingly.  
- Tools: Bootstrap, H5P, Gomo, Elucidat.  

---

### Quiz  
**Date**: Tuesday 19/11/2024  
**Time**: 11 pm  
**Duration**: 5 minutes  

**Quiz Links**:  
- **Information Systems**: [Link](https://forms.office.com/r/dwaWEyarpZ?origin=lprLink)  
- **Computer Science**: [Link](https://forms.office.com/r/ZnP4UTxSWV?origin=lprLink)  
- **Scientific Computing**: [Link](https://forms.office.com/r/5dAuCCUzEC?origin=lprLink)  
- **Computer Systems**: [Link](https://forms.office.com/r/5dAuCCUzEC?origin=lprLink)  

---

### Good Design  
"Good design is a lot like clear thinking made visual."  
– Edward Tufte