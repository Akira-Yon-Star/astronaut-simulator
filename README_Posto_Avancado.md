# Posto Avançado — Astronaut Simulator | NASA Space Apps Challenge

> An educational astronaut and space-base simulator focused on the challenges of operating a human outpost on the Moon and Mars.

**Project:** Posto Avançado  
**Challenge:** NASA Space Apps Challenge  
**Repository:** [astronaut-simulator](https://github.com/Akira-Yon-Star/astronaut-simulator)

---

## Table of contents

- [Overview](#overview)
- [Project objectives](#project-objectives)
- [Main features](#main-features)
- [Simulation structure](#simulation-structure)
- [Destinations and mission scenarios](#destinations-and-mission-scenarios)
- [Resources and base management](#resources-and-base-management)
- [Events and challenges](#events-and-challenges)
- [Technology and architecture](#technology-and-architecture)
- [NASA data and external services](#nasa-data-and-external-services)
- [How to run the project](#how-to-run-the-project)
- [Controls and accessibility](#controls-and-accessibility)
- [Educational assumptions and limitations](#educational-assumptions-and-limitations)
- [Known limitations and future improvements](#known-limitations-and-future-improvements)
- [Credits and references](#credits-and-references)

---

## Overview

Posto Avançado is an educational web-based simulator designed to introduce users to some of the challenges involved in human exploration beyond Earth. The experience combines spaceflight activities with the operation and maintenance of an outpost in an extraterrestrial environment.

The project focuses on two destinations — the Moon and Mars — and invites the player to manage essential resources, respond to environmental events, maintain infrastructure, and complete mission objectives.

The simulator is intended for learning and public engagement. Its scenarios simplify complex scientific and engineering topics so that they can be explored through an interactive experience.

## Project objectives

### General objective

Develop an interactive educational simulator that helps users understand selected challenges of astronaut missions and the operation of human bases on the Moon and Mars.

### Specific objectives

- Present key survival and infrastructure needs of an extraterrestrial outpost.
- Let users observe how resource management affects mission continuity.
- Introduce examples of environmental and equipment-related challenges.
- Provide a cockpit-style experience for selected spacecraft operation tasks.
- Make the experience accessible through multiple languages and input methods.
- Connect educational content with publicly available NASA information where supported by the application.

## Main features

- **Two exploration destinations:** Moon and Mars.
- **Multiple difficulty settings:** Training, Mission, and Survival.
- **Outpost management:** monitor essential resources and infrastructure.
- **Mission progression:** a simulated mission period of up to 20 days.
- **Environmental and technical events:** respond to changing conditions and equipment problems.
- **Cockpit experience:** interact with flight and navigation instruments in dedicated mission activities.
- **Scoring and feedback:** receive a result based on mission performance.
- **Multilingual interface:** Portuguese, English, Spanish, and French.
- **Multiple input methods:** keyboard, mouse, and compatible game controllers.
- **Fullscreen support:** use the simulator in an expanded view.

## Simulation structure

The experience is organized around two complementary activities:

1. **Outpost operations:** the user monitors the condition of the base, manages supplies, and responds to events that may affect the mission.
2. **Spaceflight activities:** the user interacts with a cockpit interface and completes selected flight-related objectives.

The exact availability and sequence of activities depend on the selected mode and the current state of the simulation.

## Destinations and mission scenarios

### Moon

The lunar scenario introduces the challenges of maintaining a human outpost on the Moon, including resource availability, energy supply, environmental exposure, and infrastructure maintenance.

### Mars

The Martian scenario explores the operation of a base in a distant environment, emphasizing the need to manage supplies, maintain equipment, and respond to environmental changes over an extended mission.

The Moon and Mars scenarios are educational representations. They should not be interpreted as operational mission plans.

## Resources and base management

The outpost simulation includes resources and systems such as:

- Oxygen
- Water
- Food
- Energy
- Health
- Equipment and spare parts
- Power generation and storage
- Oxygen production
- Water recycling
- Greenhouse systems
- Protective structures and maintenance

The purpose of these systems is to demonstrate how different parts of a base depend on one another. Resource levels and infrastructure conditions can influence the progress of the simulated mission.

## Events and challenges

During a mission, the simulator may present events that require the user to make management decisions. Examples represented in the project include:

- Solar activity and radiation-related alerts
- Micrometeorite-related incidents
- Dust and environmental interference
- Solar panel contamination or reduced performance
- Greenhouse and food-production problems
- Water leaks and recycling issues
- Communication interruptions
- Equipment and thermal-system faults

These events are simplified gameplay scenarios. Their frequency, effects, and consequences are not intended to predict real mission conditions.

## Technology and architecture

The repository currently contains the main application as a standalone HTML file:

```text
astronaut-simulator/
└── Posto_Avancado_v7_Multilingue.html
```

The application is implemented as a web page using:

- **HTML** for the page structure.
- **CSS** for layout and visual presentation.
- **JavaScript** for interface behavior and simulation logic.
- **SVG** for vector-based visual elements where used by the interface.
- **Browser storage** for local persistence of supported settings or progress.
- **Gamepad API** for compatible game-controller input.

The project is currently structured as a client-side application. No separate backend service or remote database is documented in this repository.

## NASA data and external services

The project includes informational integrations with publicly available NASA services, including:

- [NASA API Portal](https://api.nasa.gov/)
- [NASA Astronomy Picture of the Day (APOD)](https://apod.nasa.gov/apod/astropix.html)
- [NASA Image and Video Library](https://images.nasa.gov/)
- [NASA DONKI](https://api.nasa.gov/)

Availability and behavior of external services depend on their own APIs, network access, and usage limits. Where a demonstration API key is used, requests may be subject to rate limits.

NASA data panels are intended to provide context and educational information. They should not be interpreted as real-time operational telemetry or as authoritative inputs for real spacecraft or habitat operations.

## How to run the project

### Run locally

1. Download or clone this repository.
2. Open the project folder.
3. Open `Posto_Avancado_v7_Multilingue.html` in a modern web browser.
4. Allow an internet connection if you want to use features that retrieve information from external services.

Some browser features or external API requests may behave differently depending on the browser and how the file is opened. If a feature does not work locally, test the deployed version or use a local static web server.

### Run through GitHub Pages

GitHub Pages can host the project as a static website.

To publish it from the repository root:

1. Open the repository's **Settings**.
2. Select **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder.
5. Save the configuration.

For the repository root URL to load automatically, the main HTML file should be named `index.html` and placed in the selected publishing folder. If the file keeps its current name, open it through its direct GitHub Pages file path instead.

## Controls and accessibility

The application supports input through the keyboard and mouse, and includes Gamepad API support for compatible controllers. Fullscreen mode is also available.

The interface offers four language options:

- Portuguese
- English
- Spanish
- French

Controller compatibility and keyboard shortcuts may vary by browser and device. Users should consult the on-screen instructions provided by the application.

## Educational assumptions and limitations

> **Important:** Posto Avançado is an educational simulator. Its mechanics and numerical models are simplified for interaction and learning. They are not validated engineering models and must not be used to plan, operate, or assess real missions, spacecraft, life-support systems, or habitats.

The simulator abstracts complex subjects such as environmental conditions, life-support systems, energy production, resource consumption, spacecraft control, and mission risk. Real missions require validated data, specialized engineering models, safety procedures, and expert oversight.

External NASA services provide reference information, but their presence does not make the simulator an official NASA product or an operational NASA system.

## Known limitations and future improvements

Potential areas for future development include:

- Expanding explanations of the scientific concepts represented in each scenario.
- Adding more detailed in-app guidance for first-time users.
- Improving compatibility testing across browsers, screen sizes, and controllers.
- Expanding the range of mission scenarios and educational challenges.
- Improving the documentation of simulation rules and assumptions.
- Adding automated tests for important interface and simulation behaviors.

These are possible development directions and should not be interpreted as features already implemented.

## Credits and references

### Data and educational references

- [NASA Open APIs](https://api.nasa.gov/)
- [NASA Astronomy Picture of the Day](https://apod.nasa.gov/apod/astropix.html)
- [NASA Image and Video Library](https://images.nasa.gov/)
- [NASA DONKI](https://api.nasa.gov/)

### Development references

- [MDN Web Docs — HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [MDN Web Docs — CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [MDN Web Docs — JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [GitHub Pages documentation](https://docs.github.com/en/pages)

---

**Posto Avançado — NASA Space Apps Challenge**  
Educational project developed for the exploration of astronaut missions and extraterrestrial outpost operations.
