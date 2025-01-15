### System Analysis and Design  
**Software Testing**  
**ISTQB Certified Tester Foundation Level**  
- Prof. Rania Elgohary: rania.elgohary@cis.asu.edu.eg  
- Dr. Yasmine Afify: yasmine.afify@cis.asu.edu.eg  

---

### Systems Development Life Cycle (SDLC)  
[FIGURE]  
- **Implementation Phase** includes:  
  - Coding  
  - Testing  
  - Installation  
  - Documentation  
  - Training  
  - Support  

---

### Questions on Software Testing  
- Should I test my own code, or should somebody else?  
- Which code of my project should I test the most/least?  
- Can I test all possible inputs to see whether something works?  
- How do I know if I've tested well/enough?  
- What constitutes a good or bad test case method?  
- Is it good or bad if a test case fails?  
- What if a test case itself has a bug in it?  

---

### Difference between QA and QC  

| **Quality Assurance (QA)** | **Quality Control (QC)** |  
|-----------------------------|--------------------------|  
| Ensures quality in the processes by which products are developed. | Ensures quality in products by identifying defects in the actual products. |  
| Focuses on preventing defects by improving the process. | Focuses on identifying and correcting defects in the finished product. |  
| Proactive process. | Reactive process. |  
| Goal: Improve development and test processes to prevent defects. | Goal: Identify defects after product development and before release. |  
| Responsibility: Everyone on the team. | Responsibility: Specific testing team. |  
| Example: Verification. | Example: Validation/Software Testing. |  

---

### Testing Goals  
1. Demonstrate to the customer that the software meets its requirements.  
   - At least one test for every requirement in the requirements document.  
2. Discover situations where the software behaves incorrectly, undesirably, or does not conform to its specification.  
   - Root out undesirable system behavior like crashes, incorrect computations, and data corruption.  

---

### V-Model  
[FIGURE]  
- **Requirement** → **Acceptance Test**  
- **Design** → **System Test**  
- **System Design** → **Integration Test**  
- **Module Design** → **Unit Test**  
- **Coding**  

---

### Verification vs. Validation  
- **Verification**: Static process of verifying documents, design, and code to ensure they meet the conditions imposed at the start of the phase.  
- **Validation**: Dynamic process to ensure the software satisfies the customer's real requirements and expectations. Test data is entered, processed, and the output is verified against user expectations.  

---

### Static Testing Artifacts  
- Inspections  
- Requirements Specification  
- Software Architecture  
- UML Design  
- Database Models  
- Schemas  
- Program  
- System Testing Prototype  

---

### Static Testing Types  
- **Peer Review**: Author asks a peer to read, comment, and critique their work.  
- **Walkthrough**: Author presents the work artifact to others, explaining each piece.  
- **Inspection**: Formal meeting with a moderator, scribe, and reviewers. Reviewers read the material before the meeting and discuss issues during the meeting.  

---

### Dynamic Testing  
- Intended to show that a program does what it is intended to do and to discover defects before it is put into use.  
- Execute the program using artificial data (test data).  
- Check results for errors, anomalies, or non-functional attributes.  
- Can reveal the presence of errors but not their absence. Exhaustive testing is almost always impossible.  

---

### Software Testing Life Cycle (STLC)  
1. Requirement Analysis  
2. Test Planning  
3. Test Case Development  
4. Test Environment Setup  
5. Test Execution  
6. Test Closure  

---

### Functional/Dynamic Testing  
[FIGURE]  
- Design test cases  
- Prepare test data  
- Run program with test data  
- Compare results to expected outcomes  

---

### Functional Testing Types  
- Unit Testing  
- Smoke Testing  
- Integration Testing  
- System Testing  
- Regression Testing  
- Performance & Load Testing  
- User Acceptance Testing (UAT)  

---

### Component/Unit Testing  
- Testing individual components in isolation.  
- Carried out by the development team.  
- Defect testing process.  
- Components may be:  
  - Individual functions or methods within an object.  
  - Object classes with several attributes and methods.  

---

### Advantages of Unit Testing  
- Early problem identification reduces compound errors.  
- Fixing problems early is cheaper than fixing them later.  
- Easier debugging processes.  
- Developers can quickly make changes to the codebase.  
- Code reuse and migration to new projects.  

---

### Smoke Testing  
- Non-exhaustive set of tests to ensure critical functions work.  
- Executed before detailed functional or regression tests.  
- Purpose: Reject badly broken applications to save time.  
- Result determines if a build is stable enough for further testing.  
- Conducted by developers or testers.  

---

### Integration Testing  
- Testing individual units combined as a group.  
- Purpose: Expose faults in the interaction between integrated units.  
- Subfunctions may not produce the desired major function.  
- Interfacing errors not detected in unit testing may appear.  
- Timing problems in real-time systems may be detected.  

---

### Integration Testing Approaches  
[FIGURE]  
- **Decomposition-based Integration**  
  - Top-down Integration  
  - Bottom-up Integration  
  - Big-bang Integration  
- **Call-graph-based Integration**  
- **Path-based Integration**  

---

### Decomposition-based Integration  
- **Top-down Integration**: Starts with the main program, using stubs for lower-level units.  
- **Bottom-up Integration**: Starts with the leaves of the decomposition tree, using drivers.  
- **Big-bang Integration**: All components are integrated and tested at once.  

---

### System Testing  
- Focuses on a complete, integrated system to evaluate compliance with specified requirements.  
- Tests characteristics present only when the entire system is run.  
- Evaluates end-to-end system specifications.  
- Tests both functional and non-functional aspects.  
- Uses customer scenarios and usage patterns as the basis.  

---

### Regression Testing  
- Re-run all tests every time a change is made to the program.  
- Ensures changes have not broken previously working functionality.  
- Manual regression testing is expensive; automated testing is simpler.  

---

### User Acceptance Testing (UAT)  
- Users provide input and advice on system testing.  
- Essential even after comprehensive system and release testing.  
- Users have a different perspective than developers.  
- Influences from the user's working environment affect reliability, performance, usability, and robustness.  

---

### Testing Levels  
[FIGURE]  
- Unit Testing  
- Integration Testing  
- System Testing  

---

### Test Cycle Closure  
- Testing team meets to analyze testing artifacts.  
- Lessons learned are used to remove process bottlenecks for future test cycles.  
- Prepare test metrics and closure report.  
- Deliverables: Test Closure Report, Test Metrics.  

---

### Documentation  
- Testing documentation involves artifacts developed before or during testing.  
- Helps estimate testing effort, test coverage, and requirement tracking.  
- Common artifacts:  
  1. Test Plan  
  2. Test Case  
  3. Requirements Traceability Matrix  

---

### Master Test Plan  
- Developed during the analysis phase.  
- Unit, integration, and system test plans are developed during the design phase.  

---

### Test Case  
- Set of conditions and inputs used during testing.  
- Ensures software passes or fails in terms of functionality.  
- Tracks testing coverage.  
- Types: Functional, Negative, Logical, Physical, UI, etc.  

---

### Test Case Template  
[FIGURE]  
- Project Name  
- Test Case ID  
- Test Designed by  
- Test Priority  
- Module Name  
- Test Title  
- Description  
- Pre-conditions  
- Test Steps  
- Expected Results  
- Actual Results  
- Status (Pass/Fail)  

---

### Bug Report Template  
[FIGURE]  
- ID Number  
- Name  
- Reporter  
- Submit Date  
- Summary  
- URL  
- Screenshot  
- Platform  
- Operating System  
- Browser  
- Severity  
- Assigned to  
- Priority  
- Description  
- Steps to Reproduce  
- Expected Result  
- Actual Result  
- Notes  

---

### Sample Status/Progress Report  
[FIGURE]  
- Overall progress of the QA cycle  
- Total number of test cases  
- Number of tests executed  
- Number of defects encountered  
- Critical defects still open  
- Pass percentage of defects  
- Defect density  
- Critical defects percentage  

---

### Test Closure Report  
- Summary of all tests conducted.  
- Detailed analysis of bugs removed and errors found.  
- List of known issues.  
- Created by Test Lead, reviewed by stakeholders, and approved by clients.  

---

### Requirements Traceability Matrix (RTM)  
- Connects requirements throughout the validation process.  
- Ensures requirements are not lost during the project.  
- Shows the relationship between requirements and test cases.  
- Questions answered:  
  - Which test cases are affected by requirement changes?  
  - How much coverage of requirements has been achieved?  
  - Are any requirements overly complex?  

---

### RTM Example  
[FIGURE]  
- Business Requirement  
- Stakeholder Requirement  
- Functional Requirements  
- Design  
- Code  
- Test Scenario  
- Test Case  

---

### Practical Example: Test Case Writing  
[FIGURE]  
- Test Case for Facebook Login  
- Steps:  
  1. Open URL "www.facebook.com"  
  2. Enter username  
  3. Enter password  
  4. Click "Login" button  
- Expected Result: User logs in successfully and navigates to the home page.  
- Actual Result: User fails to log in, and an error message is displayed.  

---

### Bug Report Example  
[FIGURE]  
- ID: Facebook_Login_001  
- Title: User failed to log in using valid input  
- Pre-condition: URL should be accessible  
- Expected Result: User logs in successfully  
- Actual Result: User fails to log in, error message displayed  
- Severity: High  
- Priority: High  

---

### References  
- https://estb.org.eg/English/Pages/Resources/ISTQBsyllabi.aspx  
- https://www.testorigen.com/writing-an-effective-bug-report-for-a-better-software-development-process/  
- https://www.edureka.co/blog/what-is-integration-testing-a-simple-guide-on-how-to-perform-integration-testing/  

---

### Testing Levels Summary  
1. Unit Testing  
2. Integration Testing  
3. System Testing  
4. Acceptance Testing  

--- 

[End of Document]