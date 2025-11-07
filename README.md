# Improving Wireshark's User Interface
**Human-Computer Interaction Design Project | Georgia Tech CS6750**

## Overview

This project redesigned the display filter interface for [Wireshark](https://www.wireshark.org/), the world's most popular network protocol analyzer. Through a complete HCI design lifecycle, I identified usability issues affecting both novice and expert users, developed and evaluated multiple prototypes, and created a final design that showed **statistically significant improvement** (p < 0.001) over the original interface.

## The Problem

Wireshark's display filter is a critical tool for network security professionals to filter through millions of network packets. However, the existing interface presented several challenges:

- **Poor visibility of system status** - Users often couldn't tell if filters were successfully applied
- **High learning curve** - Beginners frequently made syntax errors
- **Hidden features** - Important functionality like saved filters and error messages had low discoverability

As someone who teaches network security, I repeatedly observed students struggling with these same issues.

## Design Process

### 1. Needfinding
- **Interviews** with 3 cybersecurity professionals
- **Survey** of 20 classmates (various experience levels)
- **Heuristic evaluation** using Nielsen's usability heuristics

### 2. Initial Prototyping
Created three distinct wireframe design alternatives addressing different aspects of the usability issues:

<table>
<tr>
<td width="33%">
<img src="images/1%20-%20Prototype.png" width="100%">
<b>Prototype 1</b><br/>
Focus on visual feedback and error messaging
</td>
<td width="33%">
<img src="images/2%20-%20Prototype.png" width="100%">
<b>Prototype 2</b><br/>
Split-view design with dedicated filter workspace
</td>
<td width="33%">
<img src="images/3%20-%20Prototype.png" width="100%">
<b>Prototype 3</b><br/>
Sidebar approach with filter library option
</td>
</tr>
</table>

### 3. Evaluation & Iteration
- Conducted user testing with both interviews and surveys
- Analyzed quantitative and qualitative feedback
- Identified Prototypes 1 and 2 as most promising

### 4. Final Prototype
Combined the best elements of top-performing prototypes into final wireframe:

![Final Prototype](images/Improved%20Interface%20Overview.png)

**Key Features:**
- **Enhanced visibility** - Clear visual feedback for filter status with color coding
- **Improved error messaging** - Contextual help displayed inline
- **Resizable filter workspace** - Accommodates complex filters with drag-to-resize
- **Better discoverability** - Reorganized menus and keyboard shortcuts
- **"Clear filter" button** - One-click filter removal with clear visual indicator

## Results

The final prototype was evaluated through interviews and surveys with 13 participants:

| Metric | Final Prototype | Original | p-value |
|--------|----------------|----------|---------|
| Overall Rating (1-5) | **4.17 ± 0.34** | 3.00 ± 0.38 | **< 0.001** |
| Ease of Learning (1-5) | **4.11 ± 0.29** | 2.50 ± 0.42 | **< 0.001** |
| Productivity (1-5) | **4.22 ± 0.39** | 2.55 ± 0.39 | **< 0.001** |

The design showed statistically significant improvement over the baseline interface (t = 6.62, p < 0.001).

## Design Principles Applied

- **Discoverability** - Made advanced features more visible and accessible
- **Simplicity** - Streamlined common tasks while preserving power-user functionality
- **Feedback** - Clear system status communication through visual indicators
- **Error Prevention** - Inline error messages and syntax assistance
- **Flexibility** - Resizable interface accommodating different use cases

## Technologies & Methods

- **Needfinding**: Contextual inquiry, surveys, heuristic evaluation
- **Design**: Low-fidelity wireframes, iterative prototyping
- **Evaluation**: User interviews, Likert-scale surveys, statistical analysis (t-tests, confidence intervals)
- **Tools**: Wireshark (open source network analyzer)

## Project Details

For complete methodology, analysis, and appendices, see [HCI Individual Project.md](HCI%20Individual%20Project.md).
