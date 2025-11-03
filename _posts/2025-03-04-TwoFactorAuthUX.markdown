---
layout: post
title: "Two-Factor Authentication UX Redesign at Georgia Tech"
date: 2025-03-04 10:00:00 -0500
categories: UX Design
excerpt: "Redesigned two-factor authentication using needfinding research with real survey participants. Created an interactive prototype showcasing improved user experience based on real feedback."
---

## Project Overview

For my Human-Computer Interaction (HCI) class, I led a comprehensive UX redesign project focused on improving the two-factor authentication experience. Using the HCI design lifecycle, I conducted research with real survey participants to understand pain points and user expectations. With this information, I could make prototypes, evaluate them, and iterate on this cycle. I performed two full iterations

## Process

- **Needfinding Research**: Conducted surveys with actual users to identify friction points in current 2FA implementations, using Duo as an existing interface to compare against. Needs such as less frustration and an easier process were discovered.
- **Design Alternatives**: Brainstormed ideas to solve these pain points using the best brainstorming techniques.
- **Prototypes**: I created multiple low fidelity prototypes in the first cycle and a medium-high fidelity prototype in the second cycle. Ideas prototyped included a smell-id system and a biometric only 2FA system.
- **Evaluation**: More surveys were done to evaluate the prototype against the existing interface of Duo. This feedback was used as needfinding data to create more design alternatives and choose more prototypes.

## Outcome

The final prototype showcases a better user experience for performing two-factor authentication. It was rated to have better ease and less frustration then Duo.

## Design Choices

- **Only Biometric Scanning**: This system was constrained to only use biometric scanning in order to reduce a need for a second device, which was a frustration point for users. For devices without any built-in biometric scanners, a short USB stick was prototyped to enabled fingerprint scanning on all devices.
- **Great Perceptibility**: The interface was designed to provide immediate feedback on what was happening. It was overlayed on top of the login screen to provide context on the login. It also had a progress bar when scanning starts to indicate it started and the progress of that scan.

**View the interactive prototype**: [https://morse-holly-37728409.figma.site/](https://morse-holly-37728409.figma.site/)

## Key Learnings

This project taught me how important the user is in making great user experiences. We can learn great design principles, but the best interface may violate a few of these principles. The importance of taking a step back was also proven vital here. Instead of focusing on how to improve the task of entering a code on your phone on the Duo app, I asked "why" we needed to do that. The overall reason for the task is to perform the goal of two-factor authentication. The interface becomes limitless with this broad goal instead of a focused task.