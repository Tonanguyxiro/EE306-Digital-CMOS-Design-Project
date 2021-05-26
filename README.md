# EE306 Digital CMOS Design Project

**This is the final project for EE306 Digital CMOS Design by *School of Microelectronic* (SME), *Southern University of Science and Technology* (SUSTech).**

Project Team members including YUAN Tong and FAN Qinyuan from class 2018.

## Introduction

The project contain two version, standard version and involution version. For standard version is a normal design of multiplier, for involution version, we reduce the area and delay of the multiplier by any method possible, this version can help one achive higher score but cannot be used in real world because the design in just bu-shit.

Here is a brief introduction of the project, for more details please refer to the **[Project Report(standard)](standard/Report/IEEE_report/4x4_multiplier_design.pdf)** and **[Project Report(involution)](involution/Report/IEEE_report/4x4_multiplier_design.pdf)**, we will first introduce the design of basic gates, adders and the structure of the 4x4 multiplier. Then, we will create a layout for our design. All the procedure are following the Top-to-Down design and Down-to-Top develop.

## Project Structure

### Design

In both version, we put [design files](standard/Design/multiplier), the [figure of the schematic and layout](standard/Design/Design_figures) and [simulation results](Design/simulation) in [this forder](standard/Design), the version shown here is standard version because it is more elegant.

- [Design_figures](standard/Design/Design_figures)
- [multiplier](standard/Design/multiplier)
- [simulation](standard/Design/simulation)
  - [ADE_output](standard/Design/simulation/ADE_output)
  - [test_files](standard/Design/simulation/test_files)
  - [trans_result](standard/Design/simulation/trans_result)

### Reference

Some important reference files are put here, for example, I have simplify the design rules we need in this project in file [Design_Rules.pdf](reference/Design_Rules.pdf)

### Report

Here is the Latex source code of the design 

### Addition

## Design of each level

### Design of Basic Gates

### Design of Adders

### Design of the multiplier

## Performance

### Area of the Layout

As we tested, the area of the layout is \textbf{**((0.39, -52)(62, 0)), 3276um2**}

## Propagation delay

Here we will compare the post-layout delay measurements with the schematic level delay measurement 50f F cap is attached to the output. We apply two set of input to the multiplier so we can get the transfer data of all output. The first set is $0000 \times 1111 = 11100001$ and the second set is $0010 \times 1111 = 00011110$. As we measure, the maxmun down-to-up delay is **1.915ns** for av-extracted view and **1.560ns** for schematic view, uo-to-down delay is **0.96ns** for av-extracted view and **0.773ns** for schematic view, from the data we could found that the delay of schematic view is a little lower than av-extracted view due to omiting of some cap. The plots are shown in Appendix.

## Layout Technic

Here we will introduce some layout skills that TAs will not tell you during the course, but they greatly helped me to improve the performance of the multiplier

## Conclusion

In this project, we experience the procedure of Top to Down design and Down to Top Develop, we first design the multiplier in hignest level, then we gradually split each of the component so we can get the basic logic gate we need. The development procedure start form the bisic logic gate, we design half adder and full adder based on these logic gates, finally the multiplier will be constructed by adders. In each level a serises of test were done to make sure the design functions well. During the layout procedure, we change the way transistors were put, so the size and delay is reduced.
