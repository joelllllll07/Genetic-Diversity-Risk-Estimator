# GenDiversity – Genetic Diversity Risk Estimator

## Project Overview
GenDiversity is an educational population genetics simulator built for portfolio and learning purposes.  
It demonstrates Wright–Fisher style allele-frequency dynamics and visualizes how drift, mutation, selection, and migration can influence inbreeding risk over generations.

## Features
- Wright–Fisher style simulation loop with generation-by-generation updates
- Interactive controls for population size, generations, mutation rate, selection coefficient, and initial allele frequency
- Optional migration intervention to compare baseline vs intervention outcomes
- Real-time Chart.js visualization of:
  - Allele frequency (`p`)
  - Inbreeding coefficient (`F`)
- Risk classification bands for inbreeding interpretation
- Three.js animated visual background for presentation quality

## Technologies Used
- **HTML5** for page structure
- **CSS3** for responsive styling and layout
- **Vanilla JavaScript (ES6+)** for simulation and UI logic
- **Chart.js** for data visualization
- **Three.js** for animated background rendering
- **Supabase JS client** (optional auth path) with local fallback for demo mode

## Architecture
The project is a static front-end application with two primary experiences:

1. **Landing page** (`index.html`)
   - Project positioning, educational framing, and concept overview
2. **Simulator page** (`simulator.html`)
   - Authentication UI, simulation controls, chart rendering, and summary output

Supporting legacy authentication artifacts:
- `login.html` (legacy standalone login screen)
- `auth.js` (legacy standalone authentication helper script)

## Installation Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/joelllllll07/Genetic-Diversity-Risk-Estimator.git
   ```
2. Open the project directory:
   ```bash
   cd Genetic-Diversity-Risk-Estimator
   ```
3. Run with any static web server (recommended), for example:
   ```bash
   python3 -m http.server 8000
   ```
4. Open:
   - `http://localhost:8000/index.html`

## Usage Instructions
1. Start on the landing page and open the simulator.
2. Sign in or create an account in the simulator interface.
   - If cloud auth is unavailable, demo-mode local storage fallback is used.
3. Set simulation parameters:
   - Population size (`N`)
   - Generations
   - Initial allele frequency (`p₀`)
   - Mutation rate (`μ`)
   - Selection coefficient (`s`)
4. (Optional) Enable intervention and configure migrant parameters.
5. Click **Run simulation** to generate curves and risk summary.
6. Use **Reset to defaults** to restore baseline settings.

## Screenshots
> Placeholder slots are intentionally included for portfolio readiness; replace these with real captures before sharing with recruiters.

- `docs/screenshots/landing-page.png` *(placeholder)*
- `docs/screenshots/simulator-controls.png` *(placeholder)*
- `docs/screenshots/simulation-results.png` *(placeholder)*

## Future Improvements
- Multi-run Monte Carlo mode with confidence intervals
- Exportable simulation reports (CSV/JSON/PDF)
- Parameter presets for common conservation scenarios
- Dedicated unit tests for core simulation functions
- Accessibility upgrades (keyboard navigation and ARIA refinement)

## License
This project is available under the MIT License.  
If no license file is currently present, add one before distribution.
