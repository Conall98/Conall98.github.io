---
title: "Lunar Lander Flight Simulator"
tag: "Simulation"
order: 4
description: "A Python-based six-degree-of-freedom terminal descent and landing simulator for lunar landers, driven by real LRO digital elevation maps and used to simulate landing on the rim of Shackleton crater."
image: "/assets/img/hakuto_lander.gif"
---

A Python-based six-degree-of-freedom (6-DoF) terminal descent and landing simulator for lunar landers.

The simulator models the final phase of a lunar landing — from the powered descent initiation down to touchdown — with the lander treated as a rigid body subject to thrust, gravity, and attitude control torques. Translational and rotational dynamics are integrated together so the lander's pose, velocity, and angular rates evolve consistently throughout the descent.

## Real terrain

Instead of landing on an idealised flat plane, the simulator uses **real digital elevation map (DEM) data** from NASA's **Lunar Reconnaissance Orbiter** (LRO). The terrain mesh is sampled directly from LRO LOLA altimetry, which means slopes, ridges, and crater walls are represented at the actual resolution of the spacecraft's measurements.

This matters because the touchdown environment is what kills landers — even a successful descent can end badly if the final metres put a footpad on a boulder or a 15° slope.

## Shackleton crater

The simulator has been used to model a landing on the **rim of Shackleton crater** at the lunar south pole. Shackleton is one of the most operationally interesting sites on the Moon: its rim has near-permanent sunlight (important for solar power) while the floor of the crater is in permanent shadow and is believed to hold water ice. That combination of features makes it a likely site for early crewed activity, and also makes it geometrically nasty — the rim is a high, sloped, scarred ridge with little margin for error.

Running the simulation against the real LRO DEM of the Shackleton rim shows how attitude control authority, descent velocity, and footpad placement interact with terrain features that don't appear in any simplified test case.

## What it's for

This tool was built to support concept-stage trade studies for lunar lander projects — letting you ask questions like "how much hover-time margin do we need to retarget around a boulder field?" or "what slope can this configuration land on?" without having to wait for high-fidelity flight software.
