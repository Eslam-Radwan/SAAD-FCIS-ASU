### System Analysis and Design  
#### Software Testing II  
**ISTQB Certified Tester Foundation Level**  
**Prof. Rania Elgohary**  
- Email: rania.elgohary@cis.asu.edu.eg  
**Dr. Yasmine Afify**  
- Email: yasmine.afify@cis.asu.edu.eg  

---

### Test Case Design Techniques  
- Test case design techniques are used to pick test cases in a systematic manner.  
- By using these techniques, we can save testing time and achieve good test coverage.  

---

### Black, White, and Experience-Based Testing  

#### **Black Box Testing (Based on Requirements)**  
- Tests are created from the requirements.  
- Specification models can be used for systematic test case design.  
- Techniques:  
  - Equivalence Partitioning  
  - Boundary Value Analysis  
  - Decision Tables  
  - State Transition Testing  

#### **White Box Testing (Based on Code and Design)**  
- Tests provide the ability to derive the extent of coverage of the whole application.  
- Techniques:  
  - Statement Coverage  
  - Branch Coverage  
  - Decision Coverage  

#### **Experience-Based Testing**  
- Based on the knowledge of the tester.  
- Uses past experience and intuition to "guess" where errors may occur.  
- Techniques:  
  - Error Guessing  
  - Exploratory Testing  

---

### Specification-Based (Black-Box) Testing  

#### **Equivalence Partitioning (EP)**  
- A black-box test technique to reduce the number of required test cases.  
- Steps in equivalence testing:  
  - Identify classes of inputs with the same behavior.  
  - Test at least one member of each equivalence class.  
  - Assume behavior will be the same for all members of the class.  
- Criteria for selecting equivalence classes:  
  - Coverage: Every input is in one class.  
  - Disjointedness: No input is in more than one class.  
  - Representation: If an error occurs with one member of the class, it will occur with all.  

**Example:**  
- A program accepts an integer in the range -100 to +100.  
- Equivalence partitioning:  
  - Invalid: <= -101, >= 101  
  - Valid: -100 to +100  

#### **Boundary Value Analysis (BVA)**  
- A black-box testing technique that focuses on the boundaries of input domains.  
- Reasons for using BVA:  
  - Programmers often make mistakes with boundary conditions (e.g., using <= instead of <).  
  - Requirements may not be clear around boundaries.  
- Example:  
  - Test a field that accepts amounts more than 10 and less than 20.  
  - Boundary values: 9, 10, 11, 19, 20, 21.  

#### **Decision Table Testing**  
- A precise and compact way to model complicated logic.  
- Useful for applications with:  
  - Prominent if-then-else logic.  
  - Logical relationships among input variables.  
  - Cause-and-effect relationships between inputs and outputs.  
- Each column of the decision table represents a rule.  
- Number of test cases = number of rules.  

**Example:**  
[FIGURE]  

#### **Use Case Testing**  
- Tests can be derived from use cases.  
- Each use case has preconditions and postconditions.  
- Useful for designing acceptance test cases with customer/user participation.  

**Example:**  
- Use case diagram for a coffee maker:  
[FIGURE]  

---

### Acceptance Test Cases  

| Test Case ID | Test Case Name | Test Case Description | Test Steps | Expected Result | Actual Result | Test Status (P/F) |
|--------------|----------------|-----------------------|------------|-----------------|---------------|-------------------|
| Acc01        | Waiting State   | When the coffee maker is not in use, it waits for user input. | System displays menu options. | Menu displayed correctly. |               |                   |
| Acc02        | Add a Recipe    | Only three recipes may be added to the coffee maker. | Add a recipe with unique name, price, and ingredients. | Recipe added successfully. |               |                   |
| Acc03        | Delete a Recipe | A recipe may be deleted if it exists in the list. | Choose the recipe to delete by name. | Recipe deleted successfully. |               |                   |

---

### Advantages of Black-Box Testing  
- Tests are performed from the user's point of view.  
- Unbiased testing as testers and developers work independently.  
- Suitable for testing very large systems.  
- No need for technical knowledge or language specification.  
- Test cases can be designed as soon as requirements are finalized.  

---

### White-Box Testing  
- Testers need access to the source code to identify and evaluate various paths, conditions, and potential issues.  
- Ensures all code paths are executed and the software functions as intended.  

#### **Types of White-Box Testing**  
- Unit Testing  
- Integration Testing  
- Execution Testing  
- Operations Testing  
- Mutation Testing  
- Statement Coverage  
- Branch Coverage  
- Path Coverage  

#### **Disadvantages of White-Box Testing**  
- Requires skilled testers, increasing costs.  
- Difficult to test every possible path.  
- Specialized tools like code analyzers and debugging tools are required.  

---

### Experience-Based Testing  

#### **Error Guessing**  
- Testers anticipate defects based on experience.  
- A structured approach is called "fault attack."  

#### **Exploratory Testing**  
- Concurrent test design, execution, logging, and learning.  
- Based on a test charter containing test objectives.  
- Useful when there are few or inadequate specifications.  

**Exploratory Testing Charter Example:**  
[FIGURE]  

---

### Negative vs. Positive Test Cases  

| **Negative Testing** | **Positive Testing** |
|----------------------|----------------------|
| What happens if the number of persons (weight) exceeds the specified limit? | Assumes the only specified number of persons will enter the lift. |
| What happens if someone smokes or causes a fire inside the lift? | There won't be smoke or fire inside the lift. |
| What happens if there is a power failure during operation? | There won't be a power failure during the working of the lift. |

---

### Prioritization of Test Cases  
- Goal: Reduce the set of test cases based on rational criteria.  
- Order of test execution is based on risk analysis.  
- Test cases covering the most important risks are executed first.  

---

### Bug Life Cycle  

1. **New:** When a defect is logged for the first time.  
2. **Assigned:** The bug is assigned to the development team.  
3. **Open:** The developer starts analyzing and working on the defect.  
4. **Fixed:** The developer makes necessary code changes and verifies the fix.  
5. **Pending Retest:** Testing is pending on the tester's end.  
6. **Retest:** The tester retests the changed code.  
7. **Verified:** The tester confirms the bug is fixed.  
8. **Reopen:** If the bug still exists, it is reopened.  
9. **Closed:** The bug is fixed, tested, and approved.  

**Bug Statuses:**  
- Duplicate  
- Rejected  
- Deferred  
- Not a Bug  

---

### Exercises  

1. **Testing can only show the presence of errors in a program. It cannot demonstrate that there are no remaining faults. Comment.**  
2. **List levels of functional testing.**  
3. **What is meant by inspection?**  
4. **Mention three advantages of white-box testing.**  
5. **Describe static testing types.**  
6. **Demonstrate the bug life cycle.**  
7. **User testing is essential, even when comprehensive system and release testing have been carried out. Comment.**  
8. **There is no separate user acceptance testing process in agile methods. Comment.**  
9. **List factors to choose test techniques.**  
10. **Identify software testing life cycle phases.**  

---

### References  
- [ISTQB Syllabus](https://estb.org.eg/English/pages/Resources/ISTQBsyllabi.aspx)  
- R. Chopra, *Software Quality Assurance: A Self-Teaching Introduction*. ISBN: 978-1-683921-68-4  
- [TestOrigen: Exploring the Latest Advances in White-Box Testing Techniques](https://www.testorigen.com/exploring-the-latest-advances-in-white-box-testing-techniques/)  

---

[FIGURE]  
[FIGURE]  
[FIGURE]