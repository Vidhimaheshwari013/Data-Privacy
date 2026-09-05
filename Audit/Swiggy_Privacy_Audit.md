# Data Privacy Audit of Swiggy

## 1. Introduction

Swiggy is a major online food delivery and convenience platform. This audit examines its publicly documented practices related to the collection and handling of user data.

The audit is based on publicly available information and focuses on identifying **potential privacy risks**, rather than testing Swiggy's internal systems.

## 2. Data Collection

According to Swiggy's Privacy Policy, the platform may collect different categories of information, including:

* Account information such as name, email address, mobile number and address.
* Device and technical information such as device identifiers, operating system and network information.
* Location information, including real-time location where permitted.
* Information related to the user's use of the platform.
* Information required to provide services and communicate with users.

### Potential Risk

The collection of a wide range of personal, device and location information can increase privacy exposure if the information is accessed, misused or retained unnecessarily.

**Risk Level: Medium**

### Recommendation

Swiggy should follow strong data-minimization practices by collecting only the information necessary for a specific service and providing clear controls and explanations to users.

## 3. Data Usage & Sharing

Swiggy's Privacy Policy states that collected information may be used to provide services, personalize the user experience, communicate with users, provide relevant advertisements, and meet legal requirements.

Data may also be shared with service providers and other parties involved in providing or supporting Swiggy's services.

### Potential Risk

Sharing personal information with multiple service providers and using data for personalization or advertising can increase the number of parties handling user information.

**Risk Level: Medium**

### Recommendation

Swiggy should clearly explain what categories of data are shared, the purpose of sharing, and provide users with appropriate privacy and advertising controls.

## 4. Data Storage & Security

Swiggy states that it uses technical and security measures to protect collected information. It also mentions the use of vault and tokenization services for sensitive information.

The policy states that Swiggy stores data using **Amazon Web Services (AWS)** and that the data may be stored on servers located outside India.

### Potential Risk

Using third-party cloud infrastructure and storing data across different locations can create additional privacy and data-security considerations.

Swiggy also states that internet transmission cannot be guaranteed to be completely secure.

**Risk Level: Medium**

### Recommendation

Swiggy should maintain strong encryption, access controls and monitoring, and provide clear information about how third-party cloud providers protect user data.

## 5. User Rights & Control

Swiggy's Privacy Policy allows users to request deletion of their personal data or withdraw consent by contacting Swiggy. The policy states that such requests take effect no later than five business days after receipt, subject to legal requirements.

Users can also manage certain email preferences, although some administrative, service and legal communications cannot be opted out of.

### Potential Risk

Users have privacy controls, but withdrawing consent may result in some Swiggy services becoming unavailable, and certain data may still need to be retained for legal reasons.

**Risk Level: Low**

### Recommendation

Swiggy should make privacy controls easy to find and clearly explain what data can be deleted, what may need to be retained, and how withdrawing consent affects different services.


## 6. Potential Vulnerabilities and Risks

Based on the publicly available privacy information reviewed, the following potential risks were identified:

| Potential Risk                                               | Risk Level | Recommendation                                                          |
| ------------------------------------------------------------ | ---------- | ----------------------------------------------------------------------- |
| Collection of extensive device and usage information         | Medium     | Collect only information necessary for the service.                     |
| Collection and use of location information                   | Medium     | Provide clear location controls and explain its purpose.                |
| Sharing data with service providers and advertising partners | Medium     | Clearly explain what data is shared and why.                            |
| Storage through third-party cloud infrastructure             | Medium     | Maintain strong access controls, encryption and monitoring.             |
| Risk of unauthorized access or data breach                   | High       | Continue strengthening security controls and regularly monitor systems. |

These findings represent **potential privacy risks based on publicly available information**. They do not establish that Swiggy currently has a security vulnerability or has experienced a data breach. Swiggy states that it uses technical and security measures to protect information, while also acknowledging that internet transmission cannot be guaranteed to be completely secure.

## 7. Conclusion

Swiggy collects and processes a significant amount of information to provide and personalize its services. It provides users with certain controls, including options for data deletion and withdrawal of consent.

However, areas such as extensive data collection, location information, third-party sharing, cloud storage and unauthorized-access risks require continued attention.

Overall, Swiggy demonstrates several privacy and security measures, but **greater transparency and strong data-minimization practices can further improve user privacy.**
