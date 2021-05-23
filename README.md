# EE306 Digital CMOS Design Project

**This is the final project for EE306 Digital CMOS Design by *School of Microelectronic* (SME), *Southern University of Science and Technology* (SUSTech).**

Project Team members including YUAN Tong and FAN Qinyuan from class 2018.

## Introduction

Here is a brief introduction of the project, for more details please refer to the **[Project Report](Report/IEEE_report/4x4_multiplier_design.pdf)**, we will first introduce the design of basic gates, adders and the structure of the 4x4 multiplier. Then, we will create a layout for our design. All the procedure are following the Top-to-Down design and Down-to-Top develop.

## Project Structure

### Design

We put [design files](Design/multiplier), the [figure of the schematic and layout](Design/Design_figures) and [simulation results](Design/simulation) in [this forder](Design).

- [Design_figures](Design/Design_figures)
- [multiplier](Design/multiplier)
- [simulation](Design/simulation)
  - [ADE_output](Design/simulation/ADE_output)
  - [test_files](Design/simulation/test_files)
  - [trans_result](Design/simulation/trans_result)

### Reference

Some important reference files are put here, for example, I have simplify the design rules we need in this project in file [Design_Rules.pdf](reference/Design_Rules.pdf)

### Report

### Addition

## Design of each level

### Design of Basic Gates

### Design of Adders

### Design of the multiplier

## Performance

### Area of the Layout

As we tested, the area of the layout is **((-11.2, -95)(53.2, 2)), 6246.8 um2**

## Propagation delay

Here we will compare the post-layout delay measurements with the schematic level delay measurement 50f F cap is attached to the output. We apply two set of input to the multiplier so we can get the transfer data of all output. The first set is  0000 x 1111 = 11100001 and the second set is  0010 x 1111 = 00011110. As we measure, the maxmun down-to-up delay is **1ns** and uo-to-down delay is **0.75ns**, the plots are shown in Appendix.

## Layout Technic

Here we will introduce some layout skills that TAs will not tell you during the course, but they greatly helped me to improve the performance of the multiplier

## Conclusion
