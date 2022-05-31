---
title: "Blue Prism"
description: "Creating a design system and prepping a major version transition"
date: 2022-05-23T10:24:27+01:00
draft: false
hero: './hero'
caption: 'A mock-up of a redesigned task-sequencing area of Blue Prism'
weight: 2
---

{{% section %}}

## Overview

When I joined Blue Prism, there hadn't been a dedicated UX team for the entirety of the organisation's 20 year history. I was the second person to join the newly formed UX team, reporting directly to the head of experience.

Blue Prism's software is industry-leading in [Robotic Process Automation (RPA)](https://en.wikipedia.org/wiki/Robotic_process_automation) and allows businesses to automate repetitive tasks, increasing efficiency and reducing margin for error.

As part of the UX team, I helped to instigate several major organisational changes to the way the product team worked.

{{%/ section %}}

{{% section %}}

## Creation of a design system

{{% webp name=`bp-design-system` alt=`An example of a UI component – a checkbox – as a shared, reusable Figma component, with multiple variants and themes.`%}}

* As the organisation moved away from Windows-only desktop software to the web, we pushed for a bespoke design system that was lightweight, modern, and accessible.
* We crafted a consistent design language that considered everything from colour choices (and combination of colours), fonts that were internationally consistent (for customers in Europe and Asia)
* A design backlog was generated based on user needs and use-cases. We collaboratively worked on components in Figma, then worked closely with front-end developers to ensure all requirements were met.
* Components were documented so that use cases and applications could be understand by all team members.
* As an experienced designer and developer of accessible web interfaces, I also provided examples of accessible attributes for developers.

{{% webp name=`bp-aria` alt=`An example of a new component – a combobox – with suggested ARIA attributes and keyboard control behaviour prepared for UI developers.`%}}


{{%/ section %}}

{{% section %}}

## User research programme

* To support the design and development of the first web interface, I worked with the product owner to recruit over 20 customers globally to participate in a user-centred design approach (double diamond).
* Over the course of a month, I conducted individual ethnographic studies with each customer, observing their workflows and interviewing users to establish in detail how they used the existing software.
* After analysing the behaviours of each customer, we focused on key areas that we could improve in the web, including incident management for companies with thousands of automated processes and complex scheduling of automated processes.
* For the first time in the organisation's history, we invited developers and other members of the product team to attend user sessions, and played back any key findings and quotes back to the team so that everyone better understood how the software was used in practice, and what user frustrations existed.
* With a better understanding of what we could improve for our users, we iterated over various design approaches, taking user feedback to see how they found each design, giving confidence and clarity to our development approach.

{{%/ section %}}

{{% section %}}

## Examples

### Complex process scheduling

{{% webp name=`scheduler-legacy` alt=`An example the existing scheduler user interface which, while capable, was not optimised for the complex process branching our customers demanded of it.`%}}
{{% webp name=`scheduler-proposed-draft` alt=`The first draft of a scheduler interface, built using elements of our design system, to better reflect the logic applied by our customers.`%}}

* We observed in multiple user sessions that our highest-performing customers were leveraging the software's scheduling functionality to do more than scheduling. 
* Customers were modularising their processes into groups of tasks that provided logical execution of authentication, queue-loading, spawning multiple simultaneous automations, and fault-reporting, all using an interface that was never optimally designed for this purpose.
* The sub-optimal interface meant that users had to use additional workarounds to restart failed schedules, maintain complex external documentation to understand the flow and operation of each of the scheduled automations, and, in some cases, create additional custom software to help manage the operation of these flows.
* Our proposed approach was to have an interface that better-reflected the logic our users were configuring, with the ability to "drop-in" at any point to execute tasks and quickly reconfigure each step if necessary.

### Proposing components in the design system

{{% webp name=`datepicker-basics` alt=`An explainer of datepicker use cases in the context of our software, based on research.`%}}
{{% webp name=`datepicker-variations` alt=`Extended examples of how a datepicker might function in other locales.`%}}

* Each time a component was proposed for a design system, we with a specific use-case example that was particular to the software, such as a datepicker, or combobox.
* Figma greatly simplified development, as developers could inspect elements in our design system documents and see their attributes (although after a certain point, colours, typography, and focus states and line-weights were all modular elements of our theme that developers could consume without needing to know specific values and hex numbers etc.)
* Beyond visual elements, behavioural and interactive controls were something I would document with additional slides for developers, and I would occasionally provide more detailed interactive examples using richer prototyping tools such as Framer.

{{% video name=`bp-rich-prototype` width=640 alt=`An example of a rich prototype created to demonstrate use cases of a number of components in the context of a new design.` %}}

{{%/ section %}}
