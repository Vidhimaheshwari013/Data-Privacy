# Practical 2: Privacy Impact Assessment (PIA)

## Aim

To conduct a Privacy Impact Assessment (PIA) of a new technology or system, identify potential privacy risks, and develop suitable strategies to mitigate those risks.

---

## Technology Selected

### AI-Powered Facial Recognition Attendance System

An AI-powered facial recognition attendance system uses a camera and facial recognition technology to identify students and automatically record their attendance.

---

## 1. System Overview

The proposed system captures a student's face through a camera and compares it with registered facial information. If a match is found, the system records the student's attendance along with the date and time.

### Components

* Camera
* Facial recognition software
* Student database
* Attendance database
* Teacher/Admin dashboard
* Authentication and access-control system

### Data Collected

* Student name
* Student ID
* Facial image or biometric template
* Attendance status
* Date and time
* Class/course information
* System logs

---

## 2. Purpose of Data Collection

The collected information is used to:

1. Identify students.
2. Automatically record attendance.
3. Maintain attendance records.
4. Allow teachers to view and manage attendance.
5. Reduce manual attendance work.

The biometric information should only be used for the specified attendance purpose.

---

## 3. Privacy Impact Assessment

A Privacy Impact Assessment helps identify how the system may affect the privacy of students and what controls should be implemented to reduce those risks.

---

## 4. Data Flow

```text
Student
   ↓
Camera
   ↓
Facial Recognition System
   ↓
Student Database
   ↓
Attendance Record
   ↓
Teacher/Admin Dashboard
```

The camera captures the student's face, the facial recognition system compares it with registered information, and a successful match creates an attendance record.

---

## 5. Privacy Principles

| Privacy Principle    | Application                                                                         |
| -------------------- | ----------------------------------------------------------------------------------- |
| Data Minimisation    | Only information necessary for attendance should be collected.                      |
| Purpose Limitation   | Biometric data should only be used for attendance.                                  |
| Transparency         | Students should be informed about data collection and its purpose.                  |
| Security             | Biometric and attendance data should be protected from unauthorized access.         |
| Accuracy             | Students should be able to correct inaccurate attendance records.                   |
| Retention Limitation | Data should not be stored longer than necessary.                                    |
| Accountability       | The institution should maintain records of access, decisions and privacy incidents. |

---

## 6. Privacy Risks Identified

| ID  | Privacy Risk                             | Likelihood | Impact | Risk Score | Risk Level |
| --- | ---------------------------------------- | ---------: | -----: | ---------: | ---------- |
| R1  | Unauthorized access to biometric data    |          3 |      5 |         15 | High       |
| R2  | Data breach or leakage                   |          3 |      5 |         15 | High       |
| R3  | Incorrect facial recognition             |          4 |      4 |         16 | High       |
| R4  | Use of biometric data for other purposes |          3 |      5 |         15 | High       |
| R5  | Excessive data retention                 |          3 |      4 |         12 | High       |
| R6  | Students not properly informed           |          3 |      4 |         12 | High       |
| R7  | Excessive administrator access           |          2 |      4 |          8 | Medium     |
| R8  | False matching or identity confusion     |          3 |      4 |         12 | High       |
| R9  | No alternative attendance method         |          3 |      3 |          9 | Medium     |
| R10 | Third-party/vendor access                |          2 |      5 |         10 | High       |

### Risk Calculation

```text
Risk Score = Likelihood × Impact
```

### Risk Scale

| Score | Level    |
| ----: | -------- |
|   1–4 | Low      |
|   5–9 | Medium   |
| 10–16 | High     |
| 17–25 | Critical |

---

## 7. Mitigation Strategies

### R1 & R2 — Unauthorized Access and Data Breach

* Encrypt biometric and attendance data.
* Use strong authentication.
* Implement role-based access control.
* Maintain access logs.
* Secure the database.
* Store only necessary biometric information.

### R3 & R8 — Recognition Errors

* Test the facial recognition system before deployment.
* Allow teachers to manually verify attendance.
* Provide a method to correct incorrect attendance.
* Monitor false matches and recognition failures.
* Maintain an alternative attendance method.

### R4 — Purpose Creep

* Clearly define the purpose of biometric data collection.
* Use biometric information only for attendance.
* Do not use it for unrelated monitoring or profiling.
* Conduct another privacy assessment if the purpose changes.

### R5 — Excessive Data Retention

* Define a data retention period.
* Delete biometric information when it is no longer required.
* Securely delete old records.
* Review stored data periodically.

### R6 — Lack of Transparency

Students should be informed about:

* What data is collected.
* Why it is collected.
* How it is used.
* How long it is retained.
* Who can access it.
* How they can request correction or raise concerns.

### R7 — Excessive Administrator Access

Use role-based permissions:

* **Student:** Can view their own attendance.
* **Teacher:** Can manage attendance for assigned classes.
* **Administrator:** Can manage the system.
* **IT/Security Staff:** Can access technical information only when necessary.

### R9 — No Alternative Attendance Method

An alternative attendance process should be provided for students who cannot or do not use facial recognition, according to institutional policy.

### R10 — Third-Party Access

If an external company provides the system:

* Limit vendor access.
* Include privacy and security requirements in the contract.
* Prevent unrelated use of student data.
* Require secure deletion or return of data when the service ends.

---

## 8. Privacy-by-Design Recommendations

The system should follow privacy-by-design principles:

1. Collect minimum necessary information.
2. Prefer secure biometric templates instead of unnecessary raw facial images.
3. Encrypt sensitive information.
4. Use role-based access control.
5. Maintain audit logs.
6. Implement automatic retention and deletion rules.
7. Provide clear privacy notices.
8. Provide a correction and complaint mechanism.
9. Regularly test security and recognition accuracy.
10. Review the PIA whenever the system or its purpose changes.

---

## 9. Residual Risk Assessment

After implementing the mitigation strategies, the remaining risks should be reassessed.

| Risk                  | Initial Level | Expected Residual Level |
| --------------------- | ------------- | ----------------------- |
| Biometric data breach | High          | Medium                  |
| Recognition error     | High          | Low–Medium              |
| Purpose creep         | High          | Low                     |
| Excessive retention   | High          | Low                     |
| Lack of transparency  | High          | Low                     |
| Excessive access      | Medium        | Low                     |
| Lack of alternative   | Medium        | Low                     |
| Vendor access         | High          | Medium                  |

Residual risks should be continuously monitored.

---

## 10. Overall Assessment

### Assessment: Conditionally Acceptable

The facial recognition attendance system can improve the efficiency of attendance management. However, it introduces significant privacy risks because biometric information is sensitive and difficult to replace if compromised.

The system should only be deployed after implementing appropriate security controls, limiting data collection, defining retention periods, restricting access, informing students, and providing a suitable alternative attendance method.

---

## 11. Conclusion

The Privacy Impact Assessment identified several important privacy risks associated with an AI-powered facial recognition attendance system.

The most significant risks are:

* Unauthorized access to biometric data
* Data breaches
* Incorrect facial recognition
* Misuse of biometric information
* Excessive data retention
* Third-party access

These risks can be reduced through encryption, access control, data minimisation, purpose limitation, proper retention policies, transparency, manual verification and regular privacy reviews.

Therefore, the proposed system can be considered **conditionally acceptable**, provided that the recommended privacy and security measures are implemented before deployment.

---

## Result

A Privacy Impact Assessment was successfully conducted for an AI-powered facial recognition attendance system. Potential privacy risks were identified, evaluated using likelihood and impact, and appropriate mitigation strategies were proposed.

