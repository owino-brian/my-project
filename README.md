# Project Portfolio: Interactive Graphics, Games, and Data Visualization Systems

## Overview

This repository is a collection of six independent software projects that together demonstrate a broad range of programming and computer graphics skills, spanning real-time 3D rendering, game development, systems-level programming, and modern web-based data visualization. The projects are implemented across multiple languages and platforms, including Java, C, C++, Python, and JavaScript (React), and illustrate practical applications of mathematics, physics simulation, object-oriented design, and user interface engineering.

Each project is self-contained and can be built and run independently. Together, they showcase the author's versatility across desktop application development, console-based systems programming, game engine architecture, and modern front-end analytics dashboards.

---

## Table of Contents

1. [Cosmic Explorer (Java 3D Space Exploration Game)](#1-cosmic-explorer-java-3d-space-exploration-game)
2. [3D Flying Plane Simulator (C Console Application)](#2-3d-flying-plane-simulator-c-console-application)
3. [3D Object and Scene Engine (C++)](#3-3d-object-and-scene-engine-c)
4. [Quantum Neural Intelligence Dashboard (React)](#4-quantum-neural-intelligence-dashboard-react)
5. [Space Invaders: Professional Edition (Python / Pygame)](#5-space-invaders-professional-edition-python--pygame)
6. [Architectural Building Renderer (Java 2D Graphics)](#6-architectural-building-renderer-java-2d-graphics)
7. [Technologies Used](#technologies-used)
8. [Project Goals](#project-goals)
9. [Future Improvements](#future-improvements)
10. [Author](#author)

---

## 1. Cosmic Explorer (Java 3D Space Exploration Game)

Cosmic Explorer is a Java Swing-based 3D space exploration game built from scratch without external game engine dependencies. It implements a custom 3D math library, a lightweight rendering pipeline, and a real-time game loop that runs at a fixed 60 frames per second.

**Key Features**

* Custom-built 3D vector and matrix mathematics (translation, rotation, and perspective projection)
* A procedurally generated universe featuring a central space station, orbiting planets with moons, an asteroid field, collectible energy crystals, and patrolling enemy ships
* A dedicated physics engine, particle system for visual effects such as explosions, and a basic sound system interface
* First-person camera controls with mouse-look and keyboard-based movement (WASD/arrow keys, boost, vertical thrust)
* A heads-up display (HUD) showing health, energy, score, frame rate, and a radar-style minimap
* Multithreaded game loop architecture separating update logic from rendering for consistent performance

**Controls:** WASD or arrow keys to move, mouse to look around, Space to ascend, Shift to boost, and Escape to exit.

---

## 2. 3D Flying Plane Simulator (C Console Application)

This project is a real-time 3D flight simulator rendered entirely within a Windows console window, written in C. It demonstrates low-level graphics programming without any graphics library, relying instead on a custom software rasterizer, a depth buffer, and direct manipulation of the console character grid.

**Key Features**

* A custom 3D-to-2D perspective projection pipeline with a per-pixel depth buffer for correct object occlusion
* Full 3-axis rotation (pitch, yaw, and roll) applied to a wireframe aircraft model
* Procedurally generated, continuously scrolling cloud fields and a simple animated terrain grid
* A live flight instrument panel displaying speed, altitude, fuel level, pitch, yaw, roll, an artificial horizon, and a compass with directional heading
* Real-time keyboard-driven flight controls with physics-based damping for stable handling

**Controls:** W/S to pitch, A/D to roll, Q/E to yaw, Space to accelerate, Shift or X to decelerate, and Escape to exit.

---

## 3. 3D Object and Scene Engine (C++)

This project is a modular, object-oriented 3D scene engine written in modern C++, designed to render multiple animated 3D objects within a shared console-based environment. It introduces a more structured architecture than the C flight simulator, using inheritance, smart pointers, and reusable mesh geometry.

**Key Features**

* An overloaded `Vector3` class supporting standard vector arithmetic (addition, subtraction, scalar multiplication, dot and cross products, and normalization)
* A `Matrix4x4` transformation system supporting rotation about all three axes and translation
* A reusable `Mesh` class with procedurally generated geometry, including cubes, UV spheres, and a stylized aircraft model
* A `GameObject` base class extended by specialized entities such as a continuously rotating cube, a flying plane following a smooth sinusoidal flight path with banking and pitching, and a sphere orbiting a central point
* A dedicated `Camera` class handling perspective projection of 3D world coordinates onto the 2D console viewport
* A `Renderer` class managing the screen buffer, depth buffer, and color buffer for correct visual layering

This engine demonstrates a scalable approach to real-time rendering architecture and serves as a foundation for more advanced 3D simulation projects.

---

## 4. Quantum Neural Intelligence Dashboard (React)

The Quantum Neural Intelligence Dashboard is a modern, AI-themed analytics platform built with React. It is designed to demonstrate advanced data visualization, real-time performance monitoring, predictive analytics, and immersive 3D visualization, all combined into a single cohesive and visually polished interface.

**Key Features**

* **Real-Time Analytics:** Live performance monitoring, dynamic metric updates, throughput tracking, and AI accuracy measurement, refreshed on a continuous interval.
* **Advanced Data Visualization:** Interactive line charts, area charts, radar charts, pie charts, and scatter plots built with Recharts, supporting multi-series comparison and tooltips.
* **AI Prediction Engine:** A simulated forecasting module that generates trend predictions, confidence scores, contributing factors, and trajectory analysis on demand.
* **Machine Learning Insights:** Algorithm benchmarking across accuracy, speed, and efficiency metrics, with side-by-side comparative visualization.
* **Anomaly Detection:** Simulated real-time data streaming with automated flagging of anomalous data points.
* **3D Neural Network Visualization:** A Three.js-powered particle system rendered on an HTML canvas, featuring one thousand animated, color-varied points representing an interconnected neural network, with continuous rotation and organic motion.
* **Tabbed Interface:** Organized navigation between Overview, Analytics, Predictions, and 3D Visualization sections, styled with a dark, gradient-based, glassmorphic aesthetic using Tailwind CSS.

---

## 5. Space Invaders: Professional Edition (Python / Pygame)

Space Invaders: Professional Edition is a fully featured reimagining of the classic arcade shooter, built using Python and Pygame. It expands on the original concept with layered enemy types, power-ups, particle effects, and complete game-state management.

**Key Features**

* A player-controlled starfighter with detailed multi-shape rendering (hull, cockpit, wings, and engines)
* Three distinct enemy types (basic, medium, and boss-tier), each with unique health values, point values, colors, and visual designs, arranged in a structured formation that advances and drops down at the screen edges
* A power-up system offering health restoration, rapid-fire, and temporary shield effects, each with distinct visual indicators and timers
* A dynamic particle system used for explosion effects and player damage feedback
* A scrolling starfield background for enhanced depth and atmosphere
* Complete game-state handling, including pause, game-over, and restart functionality, along with a live health bar, score counter, and level tracker
* Level progression, with a new enemy formation generated each time all enemies are defeated

**Controls:** Left/Right arrow keys or A/D to move, Spacebar to shoot, P to pause or resume, R to restart after game over, and Escape to quit.

---

## 6. Architectural Building Renderer (Java 2D Graphics)

The Architectural Building Renderer is a detailed 2D vector illustration built using Java's `Graphics2D` API. Rather than a game, this project is a demonstration of precise procedural graphics composition, depicting a fully rendered two-story residential building set within a landscaped property.

**Key Features**

* A two-story building rendered with gradient-shaded walls, a distinct ground floor and first floor, and a clearly defined foundation
* A detailed pitched roof with a tiled texture effect, a chimney, and rising smoke rendered through layered transparency
* Multiple styled windows featuring cross-mullions, glass-pane reflections, and flower boxes with individually colored blossoms
* A fully rendered entrance, including a paneled door, decorative arch, door handle, and entry steps
* A second-floor balcony complete with railings, a balcony door, and window detailing
* Decorative architectural elements, including corner stonework, ornamental pillars, and a gold-toned nameplate bearing the building's name
* A surrounding landscaped environment featuring a perimeter fence with a decorative entry gate, a garden path with stone tiles, trees, flowering bushes, and a sky containing a sun with radiating rays, clouds, and birds

This project highlights strong command of coordinate geometry, layered rendering order, gradients, and compositional design within a purely 2D graphics context.

---

## Technologies Used

* **Java** — Swing, AWT, Graphics2D (Cosmic Explorer, Architectural Building Renderer)
* **C** — Windows Console API, custom software rendering (3D Flying Plane Simulator)
* **C++** — Object-oriented design, smart pointers, custom 3D math and rendering pipeline (3D Object and Scene Engine)
* **Python** — Pygame (Space Invaders: Professional Edition)
* **JavaScript / React** — Recharts, Three.js, Lucide React, Tailwind CSS (Quantum Neural Intelligence Dashboard)

---

## Project Goals

This portfolio was developed to demonstrate a wide range of engineering capabilities, including:

* Building real-time rendering pipelines and custom 3D mathematics libraries from first principles
* Designing maintainable, object-oriented game architectures across multiple languages
* Implementing physics, collision detection, and particle-based visual effects
* Constructing modern, enterprise-style data visualization interfaces
* Producing precise, composition-driven 2D procedural graphics
* Applying consistent software engineering practices across desktop, console, and web platforms

---

## Future Improvements

* Migration of the console-based 3D projects (C and C++) to hardware-accelerated graphics APIs such as OpenGL or DirectX
* Integration of real backend APIs and live data sources into the Quantum Neural Intelligence Dashboard
* Persistent save/load systems and online leaderboards for Cosmic Explorer and Space Invaders: Professional Edition
* Expanded AI-driven enemy behavior across the game projects
* Cloud deployment and containerization of the web-based dashboard
* Automated testing coverage across all projects

---

## Author

**Owino Brian Otieno**
Researcher | Software Developer | AI Enthusiast | Data Science and Technology Professional

*Building intelligent systems and immersive experiences through code, mathematics, and design.*
