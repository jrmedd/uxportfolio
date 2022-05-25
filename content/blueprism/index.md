---
title: "Blue Prism"
description: "Creating a design system and prepping a major version transition"
date: 2022-05-23T10:24:27+01:00
draft: true
hero: './hero'
caption: 'A mock-up of a redesigned task-sequencing area of Blue Prism'
weight: 2
---

{{% section %}}

## Overview

When I joined Blue Prism, there hadn't been a dedicated UX team for the entirety of the organisation's 20 year history. I was the second person to join the newly formed UX team, reporting directly to the head of experience.

Blue Prism's software is industry-leading in Robotic Process Automation (RPA) and allows businesses to automate repetitive tasks, increasing efficiency and reducing margin for error.

As part of the UX team, I helped to instigate several major organisational changes to the way the product team worked.

{{%/ section %}}

{{% section %}}

## Creation of a design system

* As the organisation moved away from Windows-only desktop software to the web, we pushed for a bespoke design system that was lightweight, modern, and accessible.
* We crafted a consistent design language that considered everything from colour choices (and combination of colours), fonts that were internationally consistent (for customers in Europe and Asia)
* A design backlog was generated based on user needs and use-cases. We collaboratively worked on components in Figma, then worked closely with front-end developers to ensure all requirements were met.
* Components were documented so that use cases and applications could be understand by all team members.
* As an experienced designer and developer of accessible web interfaces, I also provided examples of accessible attributes for developers.

{{%/ section %}}

{{% section %}}

## User research programme

* To support the design and development of the first web interface, I worked with the product owner to recruit over 20 customers globally to participate in a user-centred design approach (double diamond).
* Over the course of a month, I conducted individual ethnographic studies with each customer, observing their workflows and interviewing users to establish in detail how they used the existing software.
* After analysing the behaviours of each customer, we focused on key areas that we could improve in the web, including incident management for companies with 1000s of automated processes and complex scheduling of automated processes.
* For the first time in the organisation's history, we invited developers and other members of the product team to attend user sessions, and played back any key findings and quotes back to the team so that everyone better understood how the software was used in practice, and what user frustrations existed.
* With a better understanding of what we could improve for our users, we iterated over various design approaches, taking user feedback to see how they found each design, giving confidence and clarity to our development approach.

{{%/ section %}}

{{% section %}}

## Examples

### Complex process scheduling

* We observed in multiple user sessions that our highest-performing customers were leveraging the software's scheduling functionality to do more than scheduling. Customers were modularising their processes into groups of tasks that provided logical execution of authentication, queue-loading, spawning multiple simultaneous automations, and fault-reporting, all using an interface that was never optimally designed for this purpose (see legacy images).
* The sub-optimal interface meant that users had to use additional workarounds to restart failed schedules, maintain complex external documentation to understand the flow and operation of each of the scheduled automations, and, in some cases, create additional custom software to help manage the operation of these flows.
* Our proposed approach was to have an interface that better-reflected the logic our users were configuring, with the ability to "drop-in" at any point to execute tasks and quickly reconfigure each step if necessary.

### Proposing components in the design system

* Each time a component was proposed for a design system, we with a specific use-case example that was particular to the software (see date picker example below)
* Figma greatly simplified development, as developers could inspect elements in our design system documents and see their attributes (although after a certain point, colours, typography, and focus states and line-weights were all modular elements of our theme that developers could consume without needing to know specific values and hex numbers etc.)
* Beyond visual elements, behavioural and interactive controls were something I would document with additional slides i na proposals to the developers, and I would occasionally provide more detailed interactive examples using richer prototyping tools such as Framer.

{{%/ section %}}
