---
title: SMS Cloud Connector
layout: project
image: "/assets/images/airship-uss-macon.jpeg"
description: SMS Cloud Connector for Eloqua
tags:
- project
- eloqua
- integration
categories:
- project
aws:
- Lambda
- RDS
- SQS
- S3
- VPC
- API Gateway
- CloudFront
- CloudMetrics
---

Since Eloqua is primarily focused on email marketing and campaign management, SMS messaages are not included as a core, native feature.
To address this, I developed for my client, a custom Eloqua application that integrates with three major SMS service providers:

* [Inmobile](https://www.inmobile.com/)
* [SMSDK](https://sms.dk/)
* [Sinch](https://sinch.com/)

In the Eloqua campaign canvas, marketers can easily select an SMS Cloud Connector component and drag it onto the campaign workflow. 
With just a few clicks, they can choose the contact field to merge and design a dynamic message template.

A key feature of this project was the integration of the Mustache templating engine. This was particularly valuable for Eloqua clients 
who had stringified JSON fields that needed to be dynamically merged into the SMS body. Mustache's templating capabilities made 
personalization and dynamic content integration seamless and efficient.

The reporting of the message status was implemented via callback method. Contacts were flagged as successful or failed based on the 
message delivery outcome and then imported back into Eloqua for tracking and reporting.

This integration streamlined the process of adding SMS to Eloqua campaigns, providing marketers with a simple, effective way to 
incorporate SMS messaging as part of their multi-channel strategies.


