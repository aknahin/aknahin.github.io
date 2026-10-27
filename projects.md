---
layout: page
title: Projects
description: >
  From routing traces across a board to guiding light into a photonic device, I approach research
  as a search for clear, testable solutions to difficult design problems.
redirect_from:
  - /projects.html
---

1. this list will be replaced by the toc
{:toc .large-only}

## Flow-field based routing algorithms for efficient PCB design automation
MS Research · 2024–2026 · KFUPM · Supervisor: Dr. Jhonathan Prieto Rojas
{:.faded}

A scalable, multilayer autorouting framework that uses cost propagation and vector fields to guide connections through complex boards. As printed circuit boards grow denser, routes must satisfy geometric constraints while balancing runtime, wirelength, and the cost of changing layers. I developed a 3D framework combining Dijkstra propagation, vector-field guidance, and via-aware costs, and integrated a U-Net model trained on the PCBench dataset to predict promising routing regions. Implemented and evaluated in Python and C++, the framework showed improved runtime efficiency and competitive routing performance on large PCB benchmarks, as described in my [CV](/assets/Asrafuzzaman-Khan-Nahin-CV.pdf).

*EDA · Pathfinding · Machine learning · Python & C++*

## High-efficiency gold bottom reflector grating coupler
BSc Research · 2022–2023 · Islamic University of Technology
{:.faded}

Exploring uneven grating geometry to couple more light into an integrated photonic device. Efficiently coupling light into photonic structures requires careful control of geometry and optical behavior, so I used ANSYS simulation tools to explore and optimize a gold bottom reflector grating coupler with uneven grating features. The optimized design increased modeled coupling efficiency from 67% to 89.5%.

*Photonics · Simulation · Optimization · ANSYS*

<div class="proj" markdown="1">

## FPGA Dynamic Robot Path Planner
{:.proj-title tabindex="0"}

<div class="pub-flyout proj-flyout" role="tooltip">
  <dl>
    <dt>Type</dt><dd>Personal project</dd>
    <dt>Tools</dt><dd>Verilog, Icarus Verilog, GTKWave, Python</dd>
    <dt>Board</dt><dd>Digilent Nexys 3 (Spartan-6 XC6SLX16)</dd>
    <dt>Code</dt><dd><a href="https://github.com/aknahin/fpga-dynamic-robot-path-planner" class="external">aknahin/fpga-dynamic-robot-path-planner</a></dd>
  </dl>
  <p>A robot starts at cell 0 of an 8×8 grid and must reach cell 63. A BFS engine in Verilog finds the shortest route using up, down, left, and right moves, and the robot follows it one cell at a time. When an obstacle lands on the part of the route it has not walked yet, the robot stops and the FPGA replans from where it stands. The board streams the robot position, obstacle map, and route over USB-UART to a Python viewer.</p>
  <p>A randomized testbench drops walls while the robot moves, about half of them on its route, and walks one block back and forth along row 4. Every route is checked against an independent shortest-path calculation.</p>
  <div class="proj-gifs">
    <figure>
      <img src="/assets/projects/fpga-path-planner-seed36.gif" width="352" height="366" loading="lazy" alt="Robot run with seed 36: the robot replans around new walls on an 8 by 8 grid">
      <figcaption>Seed 36: 20 steps, 6 replans</figcaption>
    </figure>
    <figure>
      <img src="/assets/projects/fpga-path-planner-seed46-hard.gif" width="352" height="366" loading="lazy" alt="Robot run with seed 46 and more walls: the robot replans and waits for a moving block">
      <figcaption>Seed 46, more walls: 21 steps, 11 replans</figcaption>
    </figure>
  </div>
  <p class="proj-legend">Red: robot · Green: route · Purple: blocked route · Grey: wall · Orange: moving block · Yellow: goal · Teal: visited · Blue: cells BFS explored</p>
</div>

Personal project · 2026 · Verilog, Icarus Verilog, Nexys 3
{:.faded}

Designed an 8×8 BFS path planner that updates a robot's route when an obstacle changes. Verified obstacle avoidance and replanning with a Verilog testbench and waveform simulation. Code on [GitHub](https://github.com/aknahin/fpga-dynamic-robot-path-planner).

*FPGA · Path planning · Verilog · Icarus Verilog · Nexys 3*

</div>

## Collaborate
Have a research question in mind? I'm interested in new problems across intelligent engineering systems and autonomous planning. [Start a conversation](/contact/).
