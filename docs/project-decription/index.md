---
layout: default
title: "Project Definition"
nav_order: 1
has_children: false
---

# **Project Definition**

## **Objectives:**

1. Be able to conduct the software change process;

2. Be able to write software documents (requirement specification, design document, test cases);

3. Work in the team environment;

4. Practice presentation and communication skills by software engineering.

## **Team Setup:**

This course project is team based. Students attending this course will be grouped into 4 teams (5 students per team) and focus on software maintenance of an open-source software Mango. Teams will work on 5 new features of Mango, which are provided through feature description documents.  These 5 features are supposed to include 2 easy ones, 2 medium difficult ones and 1 hard one.

Each team must choose a member as the **project leader** (with 5% bonus of the final project points). The project leader has the responsibility of managing the project and coordinating tasks. Each feature will have a **feature champion**, who will lead this feature development. Among the 5 team members, one member will be the feature champion for the two easy features. Each medium difficult feature will have a single feature champion. The hard feature will have two feature champions including the project leader and one more team member.

All documents, presentation slides, source codes and other deliverables must be uploaded to the Moodle before the due date. At the end of the semester, the team members will do a cross evaluation of contribution among each other.

Grading rules for each deliverable will be posted on Moodle assignments. Late submission will not be accepted due to the presentation schedule.

## **Feature Change Requests:**

<table>
    <tbody>
        <tr>
            <td>
                <p>
                    <strong>Feature</strong>
                </p>
            </td>
            <td>
                <p>
                    <strong>Current Behaviors</strong>
                </p>
            </td>
            <td>
                <p>
                    <strong>Expected Behaviors</strong>
                </p>
            </td>
            <td>
                <p>
                    <strong>Difficulty Level</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p>
                    <a href="../../assets/files/FR1.pdf">Two Decimal Truncation</a>
                </p>
            </td>
            <td>
                <p>
                    Mango has an interface called the watch list that allows a user to view the stored data of a set of sensors. Alternatively, each sensor can be viewed independently of one another with the “point details” interface. Both of these tools display the collected values with unnecessary precision.
                </p>
            </td>
            <td>
                <p>
                    Mango should display all values with at most two decimal places of precision. These values should be truncated, <b>not</b> rounded. This change should be made anywhere that values are displayed.
                </p>
            </td>
            <td>
                <p>
                    <strong class="label label-green">Easy</strong> (Est. 1 file; 10 LOC)
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p>
                    <a href="../../assets/files/FR2.pdf">Muted by Default</a>
                </p>
            </td>
            <td>
                <p>
                    By default, a notification sound plays by default when certain events occur, including when a sensor records a new value. This feature can be toggled by clicking the mute button on the right side of the navigation bar.
                </p>
            </td>
            <td>
                <p>
                    This feature may become useless and annoying if a large amount of sensors are constantly recording information, so it should be disabled by default. It should not be removed completely, and it should still be possible to enable and disable the notification sound.
                </p>
            </td>
            <td>
                <p>
                    <strong class="label label-green">Easy</strong> (Est. 1 file; 1 LOC)
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p>
                    <a href="../../assets/files/FR3.pdf">Change Password Bug</a>
                </p>
            </td>
            <td>
                <p>
                    When attempting to change an administrator’s password in the “Users” page, an error occurs and the password is not changed.
                </p>
            </td>
            <td>
                <p>
                    This error should be fixed, allowing an administrator’s password to be changed without an error popup appearing.
                </p>
            </td>
            <td>
                <p>
                    <strong class="label label-green">Easy</strong> - <strong class="label label-yellow">Medium</strong> (Est. 1 files; 25 LOC)
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p>
                    <a href="../../assets/files/FR4.pdf">Landing Page</a>
                </p>
            </td>
            <td>
                <p>
                    When a user’s home page is not set, they are shown the watch list page by default. This page can be set and unset using the buttons on the right side of the navigation bar.
                </p>
            </td>
            <td>
                <p>
                    Users should be shown a landing page by default. This page should include information about mango and the sensors that are being used, as well as potentially a watch list interface. This landing page should also have its own icon on the navigation bar.
                </p>
            </td>
            <td>
                <p>
                    <strong class="label label-yellow">Medium</strong> (Est. 3 files; LOC)
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p>
                    <a href="../../assets/files/FR5.pdf">Horizontal CSV</a>
                </p>
            </td>
            <td>
                <p>
                    The report page allows the user to select a set of nodes and time period to generate a report for. This report is in the form of a csv file with the notable quality that all of the user selected sensors are in the same column. These sensors are only differentiated by the “Point Name” column.
                </p>
            </td>
            <td>
                <p>
                    For ease of readability, each sensor should have its own Point Name, Time, Value, Rendered, and Annotation columns.
                </p>
            </td>
            <td>
                <p>
                    <strong class="label label-yellow">Medium</strong> (Est. 2 files; 200 LOC)
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p>
                    <a href="../../assets/files/FR6.pdf">Optimization of Run Reports</a>
                </p>
            </td>
            <td>
                <p>
                    The user can generate a report for a set of sensors across a time range in the reports page. The data is stored in a derby (sql-based) database, and the report is generated by querying it. However, this can take a long time.
                </p>
            </td>
            <td>
                <p>
                    This process should be optimized to generate the report more quickly. This can be done in part by restructuring the derby database.
                </p>
            </td>
            <td>
                <p>
                    <strong class="label label-yellow">Medium</strong> (Est. 1 file; 4 LOC)
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p>
                    <a href="../../assets/files/FR7.pdf">More Report Charts</a>
                </p>
            </td>
            <td>
                <p>
                    When generating a report, the user can choose to generate a chart for each sensor. They can then view the chart by clicking the “View Charts” button once the report is generated.
                </p>
            </td>
            <td>
                <p>
                    This feature should be improved by adding reference lines and the ability to add descriptive labels for X and Y axes. A scatter plot should also be generated.
                </p>
            </td>
            <td>
                <p>
                    <strong class="label label-red">Hard</strong> (Est. 8 files; 225 LOC)
                </p>
            </td>
        </tr>
    </tbody>
</table>

## **Grading:**

### **- _61 points (projects)_**

> **P01:** Mango Architecture Document & Presentation: 5 points
>
> **P02:** New Features Analysis (a.k.a., Requirements): 9 points
>
> **P03:** Design (Concept Location & Impact Analysis): 9 points
>
> **P04:** Test Cases & Results: 9 points
>
> **Code Inspection:** 9 points
>
>  **New Features:** 20 points (10 points/feature, your grading = (your feature/# of your features) + (sum of others’ features/# of others’ features))

### **- _9 points - Labs (3 points per lab)_**
### **- _5 points - Cross Evaluation of Contribution of Team Members_**
### **- _5 points - Attendance (10 random checkpoints, and 0.5 point per checkpoint)_**
### **- _20 points - Exam_**

## **Criteria:**
- Grading rules for each assignment will be posted on Moodle.

## **Deliverables & Schedule & Grading Rules:**

All documents, presentation slides, source codes and other deliverables must be uploaded to Moodle before the due date. Grading rules for each deliverable are shown below. Late submission will not be accepted unless the instructor has been notified with an acceptable reason (e.g., health issues, travel for academic conferences or interviews, …, on a case by case basis).

### **1 - _Mango Architecture Diagrams (Due: February 14, 2022)_**

> **(1).** You can use any tool including Mango itself to draw the UML diagrams extracted from Mango source codes. The diagrams include one static diagram (similar to C++ class diagram, called pseudo class diagram) and one activity diagram (3 points for each of them: 3 - Good, 2 - Fair, 1 - Poor). Your diagrams need to have significant improvement compared to the sample ones. Otherwise, you cannot get the points.
>
> **(2).** One-page summary explaining these two diagrams and your improvements in details is requested. (2 point)
>
> **(3).** Presentation slides are not requested. You can present based on your diagrams and the summary. (2 points)
>
> Note that the rules for the absence of presentation are the same as before.

### **2 - _Requirement Book (Due: February 21, 2022)_**

> **(1).** Requirement Book for new features (6 points per feature, and the final grading is the average points of all features)
>
> (**Very Poor:** 1 point, **Poor:** 2 point, **Fair:** 3 points, **Fair/Good:** 4 points, **Good:** 5 points, **Excellent:** 6 points)
>
> **Grading Criteria:**
>
> **Very Poor:** No difference compared to the feature change requests.
>
> **Poor:** Difference can be observed, but requirements are not itemized.
>
> **Fair:** Difference can be observed, and requirements have been itemized.
>
> **Fair/Good:** All itemized requirements are feasible, testable, concise, and clear.
>
> **Good:** Sufficient interaction with other relevant features have been included.
>
> **Excellent:** Smart, effective and user-friendly solutions have been proposed to address the feature interaction.
>
> **(2).** Presentation: 2 points (must attend the presentation to get this credit)
>
> **(3).** Feature Change Request Table: 2 points

### **3 - _Design (Concept Location & Impact Analysis) (Due: March 7, 2022)_**

> **(1).** Updating the requirement book based on the comments from the instructor (2 points): Note - you need to highlight the changes, and create the change history table to get this credit.
>
> **(2).** Updating the diagrams to support the design (1 point): Note - you cannot get this credit if your diagram updating has no connection with the needs of your concept location and impact analysis.
>
> **(3).** Presentation (2 points): You must attend the presentation to get this credit.
>
> **(4).** Feature (5 points): 5 points per feature (2 points for concept location, and 3 points for impact analysis), and "the grading = # points of total features / # of features"
>
> **(i).** Concept Location:
>
> Describing the progress of building and executing the query for your feature - 1 point
>
> Concept location result - 1 point
>
> **(ii).** Impact Analysis: Note - you must follow the methodology introduced in the lecture and take use of your static diagram, otherwise no credit will be obtained
>
> **Grading Criteria:**
>
> **Poor** - 1 point: only provide the impact analysis result and mark it on your static diagram.
>
> **Fair** - 2 points: provide the impact analysis result and mark it on your static diagram. Also, the progress and its explanation are given in detail.
>
> **Good** - 3 points: Two different coding solutions have been evaluated based on their impact analysis results, and the decision has been given based on the evaluation result. Note - if it is impossible to have 2 alternative solutions, please explain it in detail.
>
> Note that please submit your requirement book revision, static diagram revision and design document in one zip file.

### **4 - _Test Cases & Test Results (Due: March 23, 2022)_**

> **Grading (10 points in total):**
>
> **Test case and requirement book traceability table:** 1 point
>
> **Presentation:** 2 points (Note: you must attend the presentation to get this credit unless an acceptable reason has been sent to the instructor before the presentation)
>
> **Test Cases:** 4 points per feature and the final grading is the average points of all your features.
>
> **Grading Criteria:**
>
> **Excellent** - 4 points: Full coverage to all requirements has been reached, and all test cases can be considered full test cases. Note - a test case with all key elements (i.e., case ID, title, dependency, input specification, test steps, and output specification) can be considered a full test case.
>
> **Good** - 3 points: Full coverage to all requirements has been reached, and a few test cases have issues to be considered a full test case.
>
> **Fair** - 2 points: Full coverage to all requirements has been reached, and a significant number of test cases have issues in being considered full test cases.
>
> **Poor** - 1 point: Full coverage to all requirements has NOT been reached, and a significant number of test cases have issues in being considered full test cases.
>
> **Test Results:** 3 points (test results are due by March. 23, 2022 10:20am)

### **5 - _Code Inspection (Due: April 11, 2022)_**

> This assignment is due by the last class (April 11, 2022 10:20am). However, the moderator needs to submit the author's summary and reader's log before your code inspection meeting. The in-meeting log and final summary can be appended here by the due date.
>
> Please refer to our coding and code inspection preparing slides for details.

### **6 - _Features (Due: April 24, 2022)_**

> **(1).** Coding is due by Apr. 11, 2022 before the class, and all requirements need to be demonstrated in the class;
>
> **(2).** Commit all codes into the GitHub repository by Apr. 28, 2022 before the class, and a copy of source codes of mango needs to be submitted here.
>
> **(3).** Pass all test cases (the test log needs to be submitted by Apr. 28, 2022 before the class) Note: the same moodle assignment as test cases
