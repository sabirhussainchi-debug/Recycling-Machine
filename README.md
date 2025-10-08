♻️ Recycling Machine Application
📘 Overview

The Recycling Machine Application automates the process of collecting recyclable items from customers, calculating refunds, and maintaining operational records.
It supports both customers (who return recyclable items) and operators (who manage the system and monitor daily operations).
Additionally, it interacts with an external Payment System to handle refund transactions.

🎯 Purpose

The main goal of this system is to:

Encourage recycling by providing instant refunds for returned items.

Simplify refund and receipt processes.

Help operators monitor and maintain the recycling machine effectively.

Ensure accurate transaction recording and secure handling of malfunctions.

👥 Actors
Actor	Description
Customer	Returns recyclable items and requests refunds or receipts.
Operator	Manages machine operations, monitors daily activities, and handles malfunctions.
Payment System	External system responsible for processing refund payments securely.
🧩 Main Use Cases
Use Case	Description
Return Item	Customer inserts recyclable items (like bottles or cans) into the machine.
Calculate Total Refund	Calculates the total refund amount based on the type and number of returned items.
Request Receipt	Customer can request a receipt for their refund transaction.
Identify Item Type	System identifies the type of item (plastic, glass, aluminum, etc.) to calculate refund value.
Record Transaction	Records details of each transaction, including refund amount, item type, and date.
View Daily Count	Operator checks the total number of items returned in a day.
Generate Daily Report	Creates a summary report of daily transactions and refund amounts.
Update Deposit Values	Operator updates refund rates or deposit values for different item types.
Handle Malfunction	Operator diagnoses and resolves machine errors or issues.
Reset System	Operator resets the system after maintenance or malfunction.
Trigger Alarm	Activated when a system malfunction or security issue is detected.
🔄 Relationships in the Diagram
Relationship Type	Example	Description
Include (→)	Return Item → includes → Calculate Total Refund	Indicates a mandatory process that must occur as part of another use case.
Extend (---)	Handle Malfunction → extends → Trigger Alarm	Indicates an optional or conditional action that may occur in special cases.
🧠 Workflow Summary

Customer Interaction:

Customer inserts items into the recycling machine.

The system identifies the item type and calculates the refund.

A receipt may be requested, and payment is processed through the Payment System.

System Processing:

Each transaction is recorded.

Refund values are automatically updated and stored for reporting.

Operator Interaction:

Operator views daily counts and generates daily reports.

They can update deposit values, handle malfunctions, and reset the system.

If an error occurs, an alarm is triggered to alert the operator.

🏗️ System Features

Automated refund and payment processing

Daily operational monitoring

Fault detection and recovery mechanism

Integration with external payment systems

Transparent reporting for accountability

📄 Diagram Reference

The Use Case Diagram visually represents:

Actors: Customer, Operator, and Payment System

System Boundary: Recycling Machine Application

Use Cases: Functions such as returning items, generating reports, and handling malfunctions

Relationships: Include, Extend, and Actor-System interactions
