# Hero Insurance Inc. – Auto Insurance ERD Design
This project models the data requirements and business rules of Hero Insurance Inc., an auto insurance company, by developing a detailed Entity-Relationship Diagram (ERD). The purpose is to capture all critical components related to policyholders, drivers, vehicles, insurance policies, claims, and the repair process.

[Link to ERD on draw.io](https://docs.google.com/document/d/1x4-N3zaBd4s3ilHYEuRyYyArRYi4IcDXOPbBkEa2Xdc/edit?usp=sharing)

[Link to Hero Insurance Inc. Data Description]([Hero-Insurance/Hero Insurance Inc. Data Description.pdf](https://docs.google.com/document/d/1x4-N3zaBd4s3ilHYEuRyYyArRYi4IcDXOPbBkEa2Xdc/edit?usp=sharing)


## Table of Contents

  1. [Overview](#overview)

  2. [Business Rules and Key Features](#business-rules-and-key-features)

    - Policyholders

    - Vehicles

    - Policies

    - Drivers & Driving History

    - Claims

    - Repairs

    - Compensation & Payment

  3. [Entity Highlights](#entity-highlights)

  4. [Tools Used](#tools-used)

## Overview
Hero Insurance Inc. provides auto insurance policies to both individuals and organisations. The company handles complex real-world scenarios such as accident reporting, repair tracking, compensation, and policy renewal. This ERD design forms the foundation for implementing a relational database to manage the company's core operations.



## Business Rules and Key Features

  a. Policyholders
Can be individuals or organisations. For individuals, personal information is collected, including name, gender, age, occupation, marital status, and contact details. For organisations, business data such as name, industry, and annual revenue is recorded. A main contact person is associated with each organization.

  b. Vehicles
Each policy insures one vehicle, with details like registration number, make & model, VIN, condition, value, and parking location.

  c. Policies
Policies can be issued or renewed annually. Renewed policies are treated as new records but are linked to the previous policy. Policy data includes coverage details, start/end/renewal dates, premium payments, and scheduled payment plans. Each policy lists multiple authorised drivers.

  d. Drivers & Driving History
Each driver has a license number and years of experience. Historical data on past accidents and traffic violations are collected to assess risk.

  e. Claims
Claims are made when policyholders report an incident. Each claim is handled by a claims adjuster (employee) who verifies the incident and investigates the damage. Claim details include accident info, police reports, witness statements, and photos.

  f. Repairs
A single accident can involve one or more repair jobs. Each repair job may consist of multiple repair tasks, and both estimated and actual costs are recorded. Repair estimates are collected from various repair shops.

  g. Compensation & Payment
Once a claim is approved, compensation is calculated per repair job. Payments are processed directly to the policyholder, and the claim is marked as closed once all conditions are met.
Claim history is stored for every policy.

## Entity Highlights
PolicyHolder (Individual/Organisation)

Driver, DrivingExperience, TrafficViolation, DriverAccident

Vehicle

Policy, PolicySchedule, PolicyPayment, PolicyCoverage

Claim, ClaimPayment, ClaimRepairCompensation

RepairJob, RepairTask, RepairEstimate, RepairShop

Witness, PoliceReport, Employee


## Tools Used
ERD Tool: Draw.io

Notation: Crow’s Foot Notation

Database Modeling: Normalized to 3NF



