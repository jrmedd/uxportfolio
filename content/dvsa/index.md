---
title: "DVSA CVS"
description: "Designing the Driver & Vehicle Standards Agency's Commercial Vehicle Service"
date: 2022-05-23T10:24:27+01:00
draft: false
hero: './hero'
caption: 'A screenshot of the "Manage your vehicle testing" homepage'
weight: 1
---

{{% section %}}

## Overview

This is undoubtedly one of the most complex services I've ever had to work on. The DVSA is responsible for safety on Britain's roads and tests hundreds of thousands of vehicles every year to ensure they meet safety standards. The existing business processes were complex and inefficient, the existing software packages slow and outdated, and a previous supplier had failed to deliver the project, meaning we had to pull on a lot of existing loose threads to get the job done.

A large portion of this service – visible to end users under the name "Manage your vehicle testing" – passed its GOV.UK BETA service standard assessment in September 2022.

The service users include commercial customers – haulage operators and bus companies – private vehicle owners and importers, and staff members within the DVSA across multiple departments.

{{% webp name=`cvs-service-blueprint` width=640 alt=`A zoomed out look at the first draft of a CVS service blueprint` %}}

{{%/ section %}}

{{% section %}}

## Project objectives

* Provide a service compliant with the GOV.UK Service Standard to Authorised Testing Facilities (ATFs), enabling them to monitor DVSA testing activity at their sites. This service is on a GOV.UK domain and is called "Manage your vehicle testing".
* Modernise decades of legacy processes and bring all IT to a cloud-hosted solution. This includes vehicle technical and test data records, applications made by vehicle owners and operators, financial transactions, and contractual information.

{{%/ section %}}

{{% section %}}

## Creation of the "Manage your vehicle testing" service

{{% webp name=`myvt-tct` width=640 alt=`A view of "Today's completed tests" within "Manage your vehicle testing"` %}}

* ATFs are garages – often operated by bus operators or haulage companies – that enter a contract with the DVSA to provide facilities to perform tests on vehicles. They pay the DVSA for each test from an pre-funded account (PFA) that they setup with the DVSA when they become an ATF.
* Common admin activities that ATFs need to perform in order be run efficiently include: monitoring their PFA balance and topping up their account, seeing when tests are completed and what they will be charged, and searching through past transactions for their own finances. Prior to the CVS project, they have been heavily reliant on making direct contact with the DVSA in order to perform all of these, which is frustrating and inefficient for both parties.
* The service we designed provides ATFs with the ability to: view their balance and running total of tests completed today, a full breakdown of transactions, a view of today's completed tests, the ability to top-up their account, and a team member management area to add/remove other staff members within their organisation.
* The longer term aims of the service would also incorporate a previously identified user need to apply for a vehicle test, approval, or replacement certificate. These applications are often made by ATFs themselves, as well as vehicle importers and manufacturers, many of whom also hold pre-funded accounts with the DVSA to pay for these tests.

{{%/ section %}}

{{% section %}}

## A brief look at the complexity of CVS

{{% webp name=`roadmap-planning` width=640 alt=`One of many photos taken of different whiteboard planning sessions in which we attempted to breakdown a clear path to the future service` %}}

### Service overview, blueprints, and flow diagrams

* During the first phase of the project – "milestone 0" – the user-centred design team reviewed any existing research and work that was done by the previous supplier, identifying gaps and figuring out which service users we needed to interview further.
* While the users at the public-facing end of the service were our immediate priority – ATF operators, vehicle owners etc. – we also had to consider the numerous teams and systems that operated in the DVSA to support the overall service.
* We collaboratively assembled a service blueprint, showing what the desired service would look like end-to-end and front-to-back.
* Each process here was then documented in more detail e.g. the standards requirements for each vehicle and how applicants would go about certifying those requirements.
* This service blueprint would grow to encompass the context of the users a broader picture. For example, at the point at which they enter our remit, a vehicle manufacturer may have already interacted with several other government agencies such as the DVLA, VCA, and HMRC (acronyms are all over the civil service!)

{{% webp name=`branching` width=640 alt=`A zoomed out look at some of the more complex decision trees` %}}

### Manage your vehicle testing – design iteration and development of GOV.UK service

* The previous phase of the project had helped to identify the service users and their needs, resulting in the design of web portal that ATFs could use to manage testing on their sites.
* As a user-centred design team, we felt there were aspects of the existing design work that didn't marry up with the findings of the research, and gaps in the documented decision making.
* Additionally, areas of the site that had already been developed featured numerous accessibility flaws, which weren't helped by a confusing information architecture.
* As a result, we revisited the designs and A/B tested a version that seemed more consistent with research. Happily, we found our [System Usability Scale](https://en.wikipedia.org/wiki/System_usability_scale) scores improved with our changes.
* I lead the effort to ensure our service met [WCAG 2.1](https://www.w3.org/WAI/standards-guidelines/wcag/glance/) AA standard, by contributing as a web developer, manually testing using assistive technology, and planning accessibility research and our full WCAG audit.

### Multi-factor authentication research

{{% video name=`mfa-proto` width=640 alt=`A walkthrough of our authentication prototypes, created in Figma` %}}

* Users authenticating to use our service are required to use multi-factor authentication (MFA) meaning that they would require the use of a phone to confirm their identity.
* Making this journey as usable as possible as we knew our users were spread across the [digital inclusion scale](https://userresearch.blog.gov.uk/2019/02/22/reflecting-on-how-we-developed-the-digital-inclusion-scale/).
* Our designs were tested extensively with users ranging from 5 ("learning the ropes") to 8 ("confident") on the digital inclusion scale.
* We also had to ensure that our users would be able to access a phone at their workplace, as some sites struggled with phone signal and availability of individual phone lines.
* Our resulting service included an ["assisted digital"](https://www.gov.uk/service-manual/helping-people-to-use-your-service/assisted-digital-support-introduction) pathway, where users struggling to authenticate using a mobile could contact the DVSA via a landline and temporarily disable MFA.

{{%/ section %}}
