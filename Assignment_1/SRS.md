# Software Requirement Specification

## Table of Contents

- [1. Introduction](#1-introduction)
    - [1.1 Purpose](#11-purpose)
    - [1.2 Document Conventions](#12-document-conventions)
    - [1.3 Intended Audience and Reading Suggestions](#13-intended-audience-and-reading-suggestions)
    - [1.4 Project Scope](#14-project-scope)
    - [1.5 References](#15-references)
- [2. Overall Description](#2-overall)
    - [2.1 Product Perspective](#21-product-perspective)
    - [2.2 Product Features](#22-product-features)
    - [2.3 User Classes and Characteristics](#23-user-classes-and-characteristics)
    - [2.4 Operating Environment](#24-operating-environment)
    - [2.5 Design and Implementation Constraints](#25-design-and-implementation-constraints)
    - [2.6 User Documentation](#26-user-documentation)
    - [2.7 Assumptions & Dependencies](#27-assumptions-and-dependencies)
- [3. System Features](#3-system-features)
    - [3.1. Room Inventory Management](#31-room-inventory-management)
    - [3.2. Reservation Management](#32-reservation-management)
    - [3.3. Room Allocation and Assignment](#33-room-allocation-and-assignment)
    - [3.4. Payment and Billing Management](#34-payment-and-billing-management)
    - [3.5. Guest Management](#35-guest-management)
    - [3.6. Staff Management](#36-staff-management)
    - [3.7. Reporting and Analytics](#37-reporting-and-analytics)

- [4. External Interface Requirements](#4-external-interface-requirements)
    - [4.1 User Interfaces](#41-user-interfaces)
    - [4.2 Hardware Interfaces](#42-hardware-interfaces)
    - [4.3 Software Interfaces](#43-software-interfaces)
    - [4.4 Communication Interfaces](#44-communication-interfaces)
- [5. Other Nonfunctional Requirements](#5-other-nonfunctional-requirements)
    - [5.1 Performance Requirements](#51-performance-requirements)
    - [5.2 Safety Requirements](#52-safety-requirements)
    - [5.3 Security Requirements](#53-security-requirements)
    - [5.4 Software Quality Attributes](#54-software-quality-attributes)

- [6. Other Requirements](#6-other-requirements)

# 1. Introduction

## 1.1. Purpose

The purpose of this Software Requirements Specification (SRS) is to document the requirements for the development of the
OYO hotel booking system. This SRS will allow for a complete understanding of what is to be expected from the newly
introduced system which is to be constructed. The clear understanding of the system and its’ functionality will allow
for the correct software to be developed for the end user and will be used for the development of the future stages of
the project. This SRS will provide the foundation for the project. From this SRS, the Hotel Management System can be
designed, constructed, and finally tested.

This SRS will be used by the system development team which is constructing the OYO. The Project team will use the SRS to
fully understand the expectations of this OYO to construct the appropriate software.

## 1.2. Document Conventions

The document is prepared in markdown file and has github's default the font type, size, and line spacing for md files.
It has used the bold property to set the headings of the document. Standard IEEE template is the template used to
organize the appearance of the document and its flow.\
This document follows the _IEEE 830-1998_ standard for SRS.

## 1.3. Intended Audience and Reading Suggestions

**Intended Audience:**

1. Software developers and engineers involved in the design, development, and implementation of the OYO hotel booking
   system.
2. Project managers and stakeholders responsible for overseeing the development of the OYO hotel booking system.
3. Quality assurance and testing teams responsible for testing the functionality and usability of the OYO hotel booking
   system.
4. Hotel owners and managers who will be using the OYO hotel booking system to manage their hotel inventory and
   bookings.

**Reading Suggestions:**

1. Before reading this SRS, it is recommended that readers have a basic understanding of software engineering
   principles, web technologies, and hotel management.
2. Readers should also refer to the OYO website (https://www.oyorooms.com/) to gain a better understanding of the OYO
   brand, their business model, and their approach to hotel management.
3. Readers should also refer to industry standards and best practices for web development, software engineering, and
   hotel management to gain a broader perspective on the requirements and design of the OYO hotel booking system.

## 1.4. Project Scope

The OYO hotel booking system is a software system that will enable customers to search and book hotel rooms online. The
system will provide an easy-to-use interface for users to search for hotels based on their preferred location, budget,
and other criteria. The system will also provide hotel managers with an easy way to manage their room inventory,
bookings, and customer information.

## 1.5. References

- Pierre Bourque/Richard E. (Dick) Fairle, SWEBOK version 3.0. IEEE,Copyright © 2014.
- IEEE 830-1998 Standard for Software Requirements Specification
- OYO website (https://www.oyorooms.com/)

# 2. Overall

## 2.1. Product Perspective

The OYO hotel booking system will be a web-based application that will be integrated with hotel management systems to
facilitate the booking and management of hotel rooms. The system will provide an online platform for users to search for
hotels, book rooms, and make payments securely and conveniently. The system will also provide hotel managers with a
comprehensive set of tools for managing their room inventory, bookings, and customer information.

The OYO hotel booking system will be designed to be scalable and customizable to meet the needs of different hotels and
users. The system will be built using modern web technologies, such as React, Node.js, and MongoDB, to ensure high
performance, scalability, and security. The system will also be designed to be mobile-friendly and accessible on a range
of devices, including smartphones, tablets, and desktop computers.

The OYO hotel booking system will be integrated with various third-party services, such as payment gateways, email
providers, and SMS providers, to provide users and hotel managers with a seamless experience. The system will also be
designed to comply with relevant laws and regulations, such as data protection laws and payment card industry standards,
to ensure the security and privacy of user data.

## 2.2. Product Features

The OYO hotel booking system will have the following features:

- User registration and login
- Hotel room search based on location, budget, and other criteria
- Hotel room booking and payment
- Hotel room inventory management for hotel managers
- Customer information management for hotel managers
- Reporting and analytics for hotel managers

## 2.3. User Classes and Characteristics

The user classes for the OYO hotel booking system include:

### Regular users

1. **Business Travelers:** Business travelers are a key user class for the OYO hotel booking system. They typically book
   hotels for short stays and require amenities such as high-speed internet, in-room workspaces, and 24-hour room
   service. They are often price-sensitive and may book hotels in bulk for their teams.

2. **Families:** Families are another important user class for the OYO hotel booking system. They typically book hotels
   for longer stays and require amenities such as larger rooms, kitchens or kitchenettes, and family-friendly
   activities. They may also require amenities such as cribs, strollers, and other equipment for traveling with
   children.

3. **Tourists:** Tourists are a large user class for the OYO hotel booking system, particularly in popular tourist
   destinations. They typically book hotels for shorter stays and prioritize location, proximity to tourist attractions,
   and availability of local tours and activities. They may also require amenities such as luggage storage,
   transportation services, and local restaurant recommendations.

4. **Budget Travelers:** Budget travelers are a key user class for the OYO hotel booking system, particularly in
   developing countries. They typically prioritize affordability over amenities and may book shared accommodations or
   dormitory-style rooms. They may also prioritize location, choosing hotels that are close to public transportation and
   affordable restaurants.

5. **Young Adults:** Young adults are another important user class for the OYO hotel booking system, particularly for
   leisure travel. They may prioritize socializing, choosing hotels with common areas such as bars, game rooms, or
   outdoor spaces. They may also prioritize trendy or unique accommodations, such as hostels, boutique hotels, or
   eco-friendly accommodations.

6. **Senior Citizens:** Senior citizens are a growing user class for the OYO hotel booking system, particularly in
   developed countries. They may prioritize comfort, safety, and accessibility, choosing hotels with amenities such as
   wheelchair accessibility, grab bars, or medical facilities. They may also prioritize quieter accommodations, choosing
   hotels with low noise levels and comfortable bedding.

### User classifications from the Hotel side

1. **Hotel Managers:** Hotel managers are a key user class for the OYO hotel booking system. They use the system to
   manage room inventory, pricing, and promotions, and to monitor bookings and revenue. They may also use the system to
   communicate with guests, manage staff, and access reports and analytics.

2. **Housekeeping Staff:** Housekeeping staff are another important user class for the OYO hotel booking system. They
   use the system to manage room cleaning schedules, track room status and inventory, and communicate with other staff
   members. They may also use the system to report maintenance issues or request supplies.

3. **Front Desk Staff:** Front desk staff are a critical user class for the OYO hotel booking system. They use the
   system to check-in and check-out guests, manage room allocations and changes, and process payments and refunds. They
   may also use the system to manage guest requests and complaints, and to provide local recommendations and
   information.

4. **Marketing and Sales Teams:** Marketing and sales teams are important user classes for the OYO hotel booking system,
   particularly for larger hotels or hotel chains. They use the system to manage promotions and discounts, track
   customer acquisition and retention, and analyze market trends and customer behavior. They may also use the system to
   communicate with customers and manage social media and advertising campaigns.

5. **IT and Support Staff:** IT and support staff are a key user class for the OYO hotel booking system. They use the
   system to manage technical issues and system updates, provide user support and training, and ensure data security and
   privacy. They may also use the system to develop custom features or integrations and to troubleshoot system errors or
   bugs.

## 2.4. Operating Environment

The OYO hotel booking system will be web-based and will be accessible through modern web browsers on desktop and mobile
devices.

- **Hardware Requirements:** The OYO hotel booking system can be accessed via a web browser or mobile application. For
  optimal performance, it is recommended that users have a device with at least 4GB of RAM, an internet connection with
  a minimum speed of 5 Mbps, and a screen resolution of 1024x768 pixels or higher. The system is compatible with most
  modern web browsers and mobile operating systems, including Windows, MacOS, iOS, and Android.
- **Software Requirements:** The OYO hotel booking system is a web-based application that can be accessed via a web
  browser or mobile application. To use the system, users must have a modern web browser such as Google Chrome, Mozilla
  Firefox, or Apple Safari, with JavaScript enabled. The system does not require any additional software or plugins to
  be installed on the user's device.
- **Network Requirements**: The OYO hotel booking system requires an internet connection to operate. The system is
  designed to be accessible from anywhere with an internet connection, and can be used on both wired and wireless
  networks. It is recommended that users have a reliable internet connection with a minimum speed of 5 Mbps to ensure
  smooth performance.

## 2.5. Design and Implementation Constraints

1. **Compatibility**: The OYO hotel booking system must be compatible with a wide range of hardware and software
   systems, including various operating systems, web browsers, and mobile devices. This requires careful consideration
   of
   cross-platform compatibility and support for multiple devices and screen sizes.

2. **Security**: The OYO hotel booking system must be designed to ensure the security and privacy of user data,
   including personal information, payment details, and booking records. This requires implementation of secure
   protocols for data
   encryption, secure storage, and secure transmission of data.

3. **Scalability**: The OYO hotel booking system must be designed to handle large volumes of traffic and data, and to
   scale up or down as demand fluctuates. This requires consideration of cloud hosting and server infrastructure, and
   the
   ability to add or remove resources as needed.

4. **Performance**: The OYO hotel booking system must be designed to provide fast and responsive performance, with
   minimal latency and downtime. This requires careful optimization of code, database queries, and network performance,
   as well
   as implementation of caching and load balancing strategies.

5. **Accessibility**: The OYO hotel booking system must be designed to be accessible to users with disabilities,
   including visual impairments, hearing impairments, and mobility impairments. This requires implementation of
   accessibility
   features such as screen reader support, keyboard navigation, and color contrast settings.

6. **Legal and Regulatory Requirements**: The OYO hotel booking system must comply with various legal and regulatory
   requirements, including data protection laws, consumer protection laws, and payment processing regulations. This
   requires careful consideration of legal and regulatory frameworks, and implementation of appropriate policies and
   procedures to ensure compliance.

## 2.6. User Documentation

1. **User Manuals**: The OYO hotel booking system will provide user manuals that include step-by-step instructions on
   how to use the system. The manuals will cover all key features of the system and will be available in both digital
   and print formats.

2. **Online Help Center**: The OYO hotel booking system will feature an online help center that provides users with
   access to a wide range of support resources. The help center will include FAQs, troubleshooting guides, video
   tutorials, and user forums.

3. **Training Materials**: The OYO hotel booking system will offer training materials that are designed to help users
   learn how to use the system effectively. The training materials will include interactive e-learning modules,
   in-person training sessions, and webinars.

4. **Release Notes**: The OYO hotel booking system will provide release notes for each new version of the software. The
   release notes will outline new features, bug fixes, and other changes to the system, and will provide instructions on
   how to use these new features.

5. **Glossary**: The OYO hotel booking system will feature a glossary of key terms and concepts used in the system. The
   glossary will help users understand the terminology used in the system and will provide definitions and explanations
   for technical terms and jargon.

6. **User Feedback**: The OYO hotel booking system will collect user feedback on an ongoing basis and will use this
   feedback to improve the user documentation. Users will be able to submit feedback via a feedback form in the system
   or through the help center.

## 2.7. Assumptions and Dependencies

### Assumptions:

- Users will have internet access and a compatible device to access the OYO hotel booking system.
- Users will provide accurate and complete information when booking a hotel room.
- Hotels will provide accurate and up-to-date information about their room inventory, pricing, and amenities.
- Users will agree to the terms and conditions of the OYO hotel booking system and the hotel they are booking with.
- The OYO hotel booking system will comply with all relevant legal and regulatory requirements in each country where it
  operates.

### Dependencies:

- The OYO hotel booking system depends on reliable internet connectivity and server infrastructure to operate
  effectively.
- The OYO hotel booking system may depend on third-party services or software, such as payment processors, mapping
  software, or social media platforms, to function properly.
- The OYO hotel booking system may depend on external factors, such as weather events, transportation disruptions, or
  public health emergencies, which can affect hotel availability and user behavior.
- The OYO hotel booking system may depend on the availability and quality of data provided by hotels, such as room
  inventory and pricing, which can affect user satisfaction and revenue.
- The OYO hotel booking system may depend on the ability of hotels to provide a satisfactory level of service and
  amenities to users, which can affect user retention and reputation.

# 3. System Features

## 3.1. Room Inventory Management

The OYO hotel booking system should allow hotel managers to manage their room inventory in real-time. This includes
adding or removing rooms, setting room types and capacities, and defining room rates and availability.

## 3.2. Reservation Management

The OYO hotel booking system should allow guests to make reservations online or through a mobile app. Hotel managers
should be able to manage reservations in real-time, including checking availability, approving or rejecting
reservations, and managing cancellations and modifications.

## 3.3. Room Allocation and Assignment

The OYO hotel booking system should allow hotel managers to allocate and assign rooms to guests based on their
preferences and room availability. This includes assigning rooms with specific amenities, assigning rooms based on guest
loyalty or special requests, and managing room changes or upgrades.

## 3.4. Payment and Billing Management

The OYO hotel booking system should allow guests to make payments online or through a mobile app. Hotel managers should
be able to manage billing and invoicing in real-time, including setting prices and taxes, processing payments, and
issuing refunds or cancellations.

## 3.5. Guest Management

The OYO hotel booking system should allow hotel managers to manage guest information in real-time. This includes
tracking guest history, preferences, and special requests, managing loyalty programs, and communicating with guests
through the system.

## 3.6. Staff Management

The OYO hotel booking system should allow hotel managers to manage staff information in real-time. This includes
tracking staff schedules, managing staff assignments and tasks, and communicating with staff through the system.

## 3.7. Reporting and Analytics

The OYO hotel booking system should provide real-time reporting and analytics on key performance metrics such as
occupancy rates, revenue, guest satisfaction, and staff productivity. Hotel managers should be able to access these
reports through the system or through a mobile app.

# 4. External Interface Requirements

## 4.1 User Interfaces

- The OYO hotel booking system should have a user-friendly and responsive web application that allows users to easily
  search for and book hotels, view and modify bookings, and provide feedback and ratings.
- The system should also have a mobile application that provides the same functionality as the web application and is
  available on iOS and Android platforms.
- The system should be compatible with popular web browsers such as Chrome, Safari, Firefox, and Edge.

## 4.2 Hardware Interfaces

- The OYO hotel booking system should be compatible with standard hardware such as desktops, laptops, tablets, and
  smartphones.
- The system should also be compatible with peripheral devices such as printers, scanners, and credit card readers.

## 4.3 Software Interfaces

- The OYO hotel booking system should integrate with popular payment gateways such as PayPal, Stripe, and Square to
  enable
  secure and convenient payment processing.
- The system should also integrate with popular third-party applications such as Google Maps, social media platforms,
  and
  email marketing services to provide additional functionality and improve user experience.

## 4.4 Communication Interfaces

- The OYO hotel booking system should provide multiple channels for customer support, including email, phone, and live
  chat.
- The system should also integrate with messaging platforms such as WhatsApp and Facebook Messenger to enable real-time
  communication with customers.
- The system should support multiple languages and provide translation services for non-native speakers.

# 5. Other Nonfunctional Requirements

## 5.1. Performance Requirements

1. **Response Time**: The system should respond to user requests within 3 seconds.
2. **System Capacity**: The system should be able to handle up to 100,000 simultaneous users.
3. **Search Time**: The system should provide search results within 5 seconds of the user's query.
4. **System Availability**: The system should be available to users at least 99.99% of the time.
5. **Scalability**: The system should be scalable to handle a growing number of users and requests.

## 5.2. Safety Requirements

1. **Fire Safety**: The system should be designed to comply with fire safety regulations and guidelines.
2. **Health and Safety**: The system should be designed to promote the health and safety of hotel staff and guests.
3. **Emergency Procedures**: The system should have emergency procedures in place in the event of a safety or security
   incident.
4. **Risk Assessment**: The system should undergo regular risk assessments to identify and mitigate potential safety
   hazards.
5. **Compliance**: The system should comply with relevant safety regulations and standards.

## 5.3. Security Requirements

1. **User Data Protection**: The system should protect user data from unauthorized access or disclosure.
2. **Secure Authentication**: The system should use secure authentication protocols to prevent unauthorized access.
3. **Secure Transactions**: The system should use secure transaction protocols to prevent fraudulent transactions.
4. **Secure Network**: The system should be designed to prevent unauthorized access to the network infrastructure.
5. **Compliance**: The system should comply with relevant security regulations and standards.

## 5.4. Software Quality Attributes

1. **Maintainability**: The system should be designed for ease of maintenance and future enhancements.
2. **Reliability**: The system should be reliable and free from defects or errors.
3. **Reusability**: The system should be designed for reuse of code and components.
4. **Testability**: The system should be designed to be easily testable and verifiable.
5. **Portability**: The system should be designed to be easily portable across different platforms and environments.

# 6. Other Requirements

### Legal Compliance

- The system should comply with relevant laws and regulations related to online booking systems, such as the EU's
  Package Travel Directive or the US Travel Promotion Act.
- The system should comply with data protection laws, such as the General Data Protection Regulation (GDPR) or the
  California Consumer Privacy Act (CCPA).
- The system should comply with payment processing regulations, such as the Payment Card Industry Data Security
  Standards (PCI DSS).

### Multilingual Support

- The system should support multiple languages to accommodate users from different regions and countries.
- Users should be able to easily switch between languages without affecting their bookings or account information.
- The system should also support multiple currencies, with currency conversion rates that are updated in real-time.

### Integration with Third-Party Systems

- The system should be designed to integrate with third-party systems, such as payment gateways, property management
  systems, or customer relationship management (CRM) tools.
- Integration should be seamless, with data flowing between systems in real-time.
- The system should provide an open API (Application Programming Interface) that allows third-party developers to build
  custom integrations.

### Customizability

- The system should be customizable to accommodate different hotel brand standards and business needs.
- Hotel staff should be able to customize the look and feel of the booking pages, including logos, color schemes, and
  images.
- The system should also allow hotel staff to configure pricing and promotions, as well as customize reports and
  analytics.

### Mobile Responsiveness

- The system should be mobile-friendly, with responsive design that adapts to different screen sizes and devices.
- Users should be able to easily make bookings and manage their accounts from their mobile devices.
- The system should also provide a mobile app that allows users to access the booking system on the go.

### Support and Training

- The system should be supported by a dedicated support team that can assist users with technical issues, user training,
  and other inquiries.
- User documentation and training materials should be provided to help users get up to speed quickly.
- The system should also provide online help and support, including chatbots or virtual assistants that can answer
  common user questions.
