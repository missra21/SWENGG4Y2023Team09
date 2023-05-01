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

