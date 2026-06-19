# Paper Planes Corp: Lean Flow Simulator

An interactive, web-based simulation designed for Operations Management and Supply Chain coursework. This tool allows students to practically explore Lean manufacturing principles, bottleneck identification, and line balancing through a visual, dynamic interface.

## 📖 Pedagogical Overview

This simulator serves as a digital twin for the classic "Paper Planes" physical classroom exercise. It models a four-stage unoptimised "Push" assembly line with distinct cycle times and micro-movements. 

It is specifically designed to facilitate assessments and practical workshops covering:
* **Bottleneck Analysis:** Visually demonstrating how unbalanced cycle times lead to Work-In-Progress (WIP) queue accumulation.
* **Little’s Law ($L = \lambda W$):** Allowing students to calculate and observe the relationship between WIP, throughput, and lead time.
* **Line Balancing (Heijunka):** Enabling students to reallocate cycle times across workstations to achieve continuous flow.
* **Push vs. Pull Systems:** Serving as a baseline 'As-Is' state for students to conceptually redesign into a Kanban-driven 'Pull' system.
* **Process Variation:** Introducing random "special orders" (orange paper) to demonstrate the impact of product variation on standard flow.

## ✨ Features

* **Zero Dependencies:** Built entirely with plain HTML, CSS, and Vanilla JavaScript. It requires no external libraries, databases, or server-side processing.
* **Real-Time Dashboard:** Tracks the simulation clock, total system WIP, and throughput (finished planes) dynamically.
* **Interactive Sliders:** Students can adjust the cycle time (in seconds) for each of the four operators to test different line-balancing theories.
* **Visual Queueing:** If a downstream workstation is slower than its predecessor, items visibly stack in a WIP buffer, instantly highlighting the system bottleneck.

## 🚀 Deployment and Usage

Because this tool is entirely client-side, it is exceptionally easy to host and embed into Learning Management Systems (LMS) such as Canvas, Blackboard, or Moodle.

### Embedding into an LMS (Canvas)
Do not upload the HTML file directly to Canvas file storage, as the LMS previewer will strip the JavaScript required to run the simulation. Instead, embed the live GitHub Pages link into an Assignment or Page using an iframe:

```html
<iframe src="[[https://your-username.github.io/repo-name/paper-planes-sim.html](https://nshukla-git.github.io/om-simulations/index.html)]([https://your-username.github.io/repo-name/paper-planes-sim.html](https://nshukla-git.github.io/om-simulations/index.html))" width="100%" height="750px" style="border:none;"></iframe>
