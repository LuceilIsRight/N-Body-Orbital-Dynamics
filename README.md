## N-Body Orbital Dynamics

A Python project exploring orbital dynamics through numerical simulation and visualisation.

The project uses REBOUND and Matplotlib to investigate gravitational systems and render particle trajectories. It is intended as a computational physics project, with an emphasis on making the simulated behaviour observable and the implementation easier to explore.

---

# Contents

- "Overview" (#overview)
- "Features" (#features)
- "Preview" (#preview)
- "Technology Stack" (#technology-stack)
- "Installation" (#installation)
- "Running the Project" (#running-the-project)
- "Configuration" (#configuration)
- "Scientific Considerations" (#scientific-considerations)
- "Limitations" (#limitations)
- "Roadmap" (#roadmap)
- "Contributing" (#contributing)
- "Licence" (#licence)

---

# Overview

Gravitational systems provide a practical way to explore numerical integration, initial conditions, orbital motion, and the challenges of simulating interacting bodies.

This project uses computational methods to evolve a system and visualise the resulting trajectories. It can serve as a starting point for experiments involving orbital configurations and numerical behaviour.

---

# Features

The repository has been developed around the following capabilities. Verify each against the current source before treating it as a guaranteed feature of a particular release.

- Gravitational orbital simulation using REBOUND.
- Visualisation of particle trajectories using Matplotlib.
- Configurable simulation initial conditions.
- Animation-based inspection of the simulated motion.
- Optional three-dimensional visualisation, where supported by the script.
- Video export, where supported by the installed rendering tools and current script configuration.

Preview

Add a screenshot or GIF from an actual run here.

<!-- Replace the placeholder below with a committed image or GIF. --><!-- Example: ![Orbital simulation](docs/images/orbital-simulation.gif) -->Suggested preview: a short animation showing the initial configuration and resulting orbital trajectories.

Technology Stack

Technology| Purpose
Python| Main programming language
REBOUND| N-body simulation framework
NumPy| Numerical arrays and calculations, where used
Matplotlib| Plotting and visualisation
FFmpeg| Video encoding, if the animation is exported to MP4

Installation

1. Clone the repository

git clone https://github.com/LuceilIsRight/N-Body-Orbital-Dynamics.git
cd N-Body-Orbital-Dynamics

2. Create a virtual environment

Windows (PowerShell):

py -m venv .venv
.\.venv\Scripts\Activate.ps1

Linux/macOS:

python3 -m venv .venv
source .venv/bin/activate

3. Install dependencies

Install the dependencies required by the current source code. For a project using REBOUND and Matplotlib, the basic packages may be installed with:

python -m pip install --upgrade pip
python -m pip install rebound numpy matplotlib

If the current script imports additional packages, install those as well. A committed "requirements.txt" is preferable once the environment has been tested.

Running the Project

Run the repository's main simulation script from the project directory.

For example, if the entry-point file is named "orbital_simulation.py":

python orbital_simulation.py

Check the actual filename before running this command. If the script uses a different name, replace it with the correct entry point.

Follow the prompts or configuration options implemented by the program. Output filenames and supported options depend on the current version.

Configuration

Document the configuration variables actually exposed by the source code here.

Typical parameters for an orbital simulation may include:

Parameter| Description
Initial positions| Starting locations of the simulated bodies
Initial velocities| Starting velocities
Masses| Mass assigned to each body
Integration settings| Numerical method and timestep, if configurable
Duration| Length of the simulated evolution
Visualisation settings| View, animation frame rate, and output resolution

These are general categories, not a guarantee that the current script exposes every parameter.

Scientific Considerations

Numerical simulations are sensitive to initial conditions, integration settings, and the assumptions used to construct the system.

When using the project for quantitative analysis:

- Check that the integration method is appropriate for the system.
- Investigate sensitivity to the timestep.
- Examine relevant conserved quantities when the model permits it.
- Distinguish visual plausibility from numerical accuracy.
- Record the configuration used to generate a result.

Limitations

The project's accuracy and physical scope depend on the implemented equations, numerical integrator, initial conditions, and validation performed.

Do not interpret a visually plausible orbit as proof that a system is physically stable or quantitatively accurate without suitable tests.

# Roadmap

Potential future improvements — not claims about completed functionality:

- [ ] Document a reproducible example configuration.
- [ ] Add automated tests for core calculations.
- [ ] Add numerical convergence checks.
- [ ] Document relevant conservation diagnostics.
- [ ] Separate simulation logic from visualisation logic.
- [ ] Add example outputs and a concise scientific report.
- [ ] Add a tested dependency file and continuous integration.

Contributing

Issues and suggestions are welcome. Before contributing, please describe the proposed change and how it can be tested.

Licence

Check the repository for an existing licence before reusing or redistributing this code. If no licence is present, reuse permissions should not be assumed.
