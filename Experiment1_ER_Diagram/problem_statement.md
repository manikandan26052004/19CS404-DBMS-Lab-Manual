# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.

---

## 🧪 Choose One Scenario:

### 🔹 Scenario 1: University Database
Design a database to manage students, instructors, programs, courses, and student enrollments. Include prerequisites for courses.

**User Requirements:**
- Academic programs grouped under departments.
- Students have admission number, name, DOB, contact info.
- Instructors with staff number, contact info, etc.
- Courses have number, name, credits.
- Track course enrollments by students and enrollment date.
- Add support for prerequisites (some courses require others).

---

### 🔹 Scenario 2: Hospital Database
Design a database for patient management, appointments, medical records, and billing.

**User Requirements:**
- Patient details including contact and insurance.
- Doctors and their departments, contact info, specialization.
- Appointments with reason, time, patient-doctor link.
- Medical records with treatments, diagnosis, test results.
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name

## Scenario Chosen:
 Hospital Database

## ER Diagram:
![image](https://github.com/user-attachments/assets/f166bc29-b4ec-43ff-98ef-0ef1b75cc6cd)

## Entities and Attributes:
 Patient: Age, Name, Gender, Phone No, Appointment No

Appointment: Appointment No, Duration, Online/Offline, Time, Date

 Doctor: Phone No, Mail ID, D.ID, Name, Specialization

Department: Dept Block, Dept Location, Dept ID, Dept Name

## Relationships and Constraints:
Patient ↔ Appointment (1:N, Partial Participation by Patient, Full Participation by Appointment)

Doctor ↔ Appointment (1:N, Full Participation by Doctor, Partial Participation by Appointment)

Doctor ↔ Department (1:N, Full Participation by Department, Partial Participation by Doctor)

## Extension (Prerequisite / Billing):
Prerequisites: Modeled as a Many-to-Many relationship (M:N) between entities (e.g., Course ↔ Prerequisite).

Billing: Patient ↔ Billing is One-to-Many (1:N) with Full Participation by Billing and Partial by Patient.

## Design Choices:
The entities, relationships, and assumptions were chosen to reflect real-world hospital operations. Entities like Patient, Doctor, Appointment, and Billing are essential for capturing critical details, while relationships (e.g., Patient ↔ Appointment as 1:N) mirror real-world interactions. Assumptions, such as unique IDs for Patients and Doctors and one Department hosting multiple Doctors, ensure the design remains logical, consistent, and adaptable for practical use.

## RESULT
The experiment showed the system effectively modeled entities and relationships, ensuring logical data flow and real-world applicability.
