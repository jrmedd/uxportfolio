---
title: "Emojinal"
description: "Exploring research on the sentiment of emoji"
date: 2022-05-23T13:25:15+01:00
draft: false
weight: 6
---

## Overview

Emojinal is an ongoing experiment that I created after running a series of discovery workshops with customers in Miro. As part of these workshops, we started to plot out the steps of a user journey. Once the basic framework of the journey was created, I invited the users to add post-its to the journey to summarise their mood and emotional response at each stage. To my surprise, some users responded by adding emojis to the journey. To my continued surprise, we collectively seemed to understand as a group what sentiment was being evoked by each response, suggesting we each shared a bilingual ability to read these and translate these visual markers immediately.

## Translating emotion in software

Shortly after running these workshops, I was writing a basic program that would convert Miro boards into web pages that organised the content according to the colour, position, and grouping of post-its used in each Miro board, meaning links could be shared without granting Miro access, and content could be further annotated, tagged, and searched in an application. In this program, I wanted a way of creating conventional user journey diagrams, with a mood meter than rose and fell according to mood captured in the workshop.

It was then that I realised that, while there was precedent in computing for performing sentiment analysis on text, I wasn't aware of any existing software solutions for analysing emojis in the same way. Me being me, I thought this was a gap that needed plugging!

## The Emojinal API

One of the most comprehensive studies of emoji sentiment I was a able to locate at the time was a study performed by Institut "Jožef Stefan", in Slovenia, which performed a massive analysis of the sentiment of emojis associated with tweets. Using the data generated from this study, I created an API to query this dataset by passing in emojis.

## What next?

Emojinal is an experiment I'm keen to continue exploring as a UX designer. Having successfully deployed the API in an alpha prototype, I'm keen to continue exploring our use of emojis, their relationship to language, and how we collectively understand the meanings that they offer. My hope is that future studies will improve understanding of emojis, and as number of emojis continues to expand, we'll find new and interesting ways to communicate by using them, not just our moods, but complex ideas and expressions.
