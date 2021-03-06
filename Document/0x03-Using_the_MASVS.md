# Using the Mobile Application Security Verification Standard

The MASVS can be used to establish a level of confidence in the security of mobile apps. The requirements were developed with the following objectives in mind:

* Use as a metric - To provide application developers and application owners with a framework wich allows to measure the security, and thus the degree of trust that can be placed in their mobile applications.
* Use as guidance - To provide guidance in regards to security controls necessary to implement in order to satisfy application security requirements
* Use during procurement - Provide a baseline for mobile app security verification requirements.

Figure 1 - Uses of MASVS for organizations and tool/service providers

## Mobile Application Security Verification Levels

The Mobile Application Security Verification Standard defines five security verification levels, with each level increasing in depth.

### MASVS Level 1 - Standard Security

An application that achieves MASVS level 1 adheres to mobile application security best practices. It fulfills basic requirements in terms of code quality, handling of sensitive data, and interaction with the mobile environment. A testing process must be in place to verify the security controls. This level is appropriate for all mobile applications.

### MASVS Level 2 - Defense-in-Depth

Level 2 introduces advanced security controls that go beyond the standard requirements. To fulfill level 2, a threat model must exist, and security must be considered during the design phase. This level is appropriate for applications that handle sensitive data, such as mobile banking.

### MASVS Level 3 - Defense-in-Depth and Resiliency

In addition to state-of-the-art security and defense-in-depth, level 3 defines mechanisms that increase the cost of reverse engineering the application. It can be applied to add an additional layer of protection for applications that process sensitive data. Vendors may also opt to fulfill these requirements as a means of protecting intellectual property.

### MASVS Level 4 - Defense-in-Depth and Strong Resiliency

An application that achieves MASVS level 4 has both state-of-the-art security controls and software protection. Such an application is highly resilient against attacks and reverse engineering attempts. Level 4 is meant to be applied to applications that handle highly sensitive data. Vendors may also opt to fulfill these requirements as a means of protecting intellectual property.

## How to use this standard

One of the best ways to use the Mobile Application Security Verification Standard is to use it as blueprint to create a secure coding checklist specific to your application, platform or organization. Tailoring the MASVS to your use cases will increase the focus on the security requirements that are most important to your projects and environments.

## Applying MASVS in Practice

Different threats have different motivations. Some industries have unique information and technology assets and domain specific regulatory compliance requirements.

Below we provide industry-specific guidance regarding recommended MASVS levels. Although some unique criteria and some differences in threats exist for each industry, a common theme throughout all industry segments is that opportunistic attackers will look for any easily exploitable vulnerable applications, which is why MASVS Level 1 is recommended for all applications regardless of industry. (... todo ...)

| Industry | Threat Profile | L1 Recommendation | L2 Recommendation | L3 Recommendation | L4 Recommendation |
| --- | --- | --- | --- | --- | --- |
| Finance and Insurance | Although this segment will experience attempts from opportunistic attackers, it is often viewed as a high value target by motivated attackers and attacks are often financially motivated. Commonly, attackers are looking for sensitive data or account credentials that can be used to commit fraud or to benefit directly by leveraging money movement functionality built into applications. Techniques often include stolen credentials, application-level attacks, and social engineering. Some major compliance considerations include Payment Card Industry Data Security Standard (PCI DSS),Gramm Leech Bliley Act and Sarbanes-Oxley Act (SOX). | All mobile apps. | Apps that enable access to Personally Identifiable Information. | Apps that enable access to highly sensitive information like credit card numbers, personal information, or that can move limited amounts of money in limited ways. Examples include: (i) transfer money between accounts at the same institution or(ii) a slower form of money movement (e.g. ACH) with transaction limits or(iii) wire transfers with hard transfer limits within a period of time. | Apps that enable access to large amounts of sensitive information or that allow either rapid transfer of large sums of money (e.g. wire transfers) and/or transfer of large sums of money in the form of individual transactions or as a batch of smaller transfers.
| Manufacturing, professional, transportation, technology, utilities, infrastructure, and defense | These industries may not appear to have very much in common, but the threat actors who are likely to attack organizations in this segment are more likely to perform focused attacks with more time, skill, and resources. Often the sensitive information or systems are not easy to locate and require leveraging insiders and social engineering techniques. Attacks may involve insiders, outsiders, or be collusion between the two. Their goals may include gaining access to intellectual property for strategic or technological advantage. We also do not want to overlook attackers looking to abuse application functionality influence the behaviour of or disrupt sensitive systems. Most attackers are looking for sensitive data that can be used to directly or indirectly profit from to include personally identifiable information and payment data. Often the data can be used for identity theft, fraudulent payments, or a variety of fraud schemes. | All mobile apps. | Apps that enable access to internal information or information about employees that may be leveraged in social engineering. | Apps that enable access to nonessential, but important intellectual property or trade secrets.| Apps that enable access to valuable intellectual property, trade secrets, or government secrets (e.g. in the United States this may be anything classified at Secret or above) that is critical to the survival or success of the organization. Applications controlling sensitive functionality (e.g. transit, manufacturing equipment, control systems) or that have the possibility of threatening safety of life.
| Healthcare | Most attackers are looking for sensitive data that can be used to directly or indirectly profit from to include personally identifiable information and payment data. Often the data can be used for identity theft, fraudulent payments, or a variety of fraud schemes.For the US healthcare sector, the Health Insurance Portability and Accountability Act (HIPAA) Privacy, Security, Breach Notification Rules and Patient Safety Rule ( [http://www.hhs.gov/ocr/privacy/](http://www.hhs.gov/ocr/privacy/)= [.](http://www.hhs.gov/ocr/privacy/) | All mobile apps | Apps that enable access to small or moderate amounts of Personally Identifiable Information. | Apps that enable access to sensitive medical information (Protected Health Information), Personally Identifiable Information, or payment data.| Apps used to control medical equipment, devices, or records that may endanger human life. Payment and Point of Sale systems (POS) that contain large amounts of transaction data that could be used to commit fraud. 
| Retail, food, hospitality | Many of the attackers in this segment utilize opportunistic "smash and grab" tactics. However, there is also a regular threat of specific attacks on applications known to contain payment information, perform financial transactions, or store personally identifiable information. Although less likely than the threats mentioned above, there is also the possibility of more advanced threats attacking this industry segment to steal intellectual property, gain competitive intelligence, or gain an advantage with the target organization or a business partner in negotiations. | All mobile apps. | Suitable for apps that enable access to business applications, product catalogue information, internal corporate information, and applications with limited user information (e.g. contact information). | Apps that enable access to highly sensitive information or business applications. | Payment and Point of Sale systems (POS) that process large amounts of transaction data that could be used to commit fraud. Applications that enable access to a large volume of sensitive information like full credit card numbers, mother's maiden name, social security numbers etc. 
