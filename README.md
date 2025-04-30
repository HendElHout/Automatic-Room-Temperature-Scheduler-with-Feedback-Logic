# 🌡️ Automatic Room Temperature Scheduler Simulation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)

A simulation of a smart thermostat system that automatically adjusts room temperature based on a predefined schedule using a simple feedback control mechanism.

## ✨ Features

*   **📅 Time-Based Scheduling:** Defines different target temperatures (setpoints) for various times of the day (Morning, Work Hours, Evening, Night).
*   **🌡️ Environment Simulation:** Simulates changes in room temperature considering heating, cooling, or idle states.
*   **⚙️ Feedback Control:** Implements a basic feedback loop to activate heating or cooling when the actual temperature deviates significantly from the setpoint.
*   **📊 Visualization:** Generates a plot showing the actual temperature vs. the setpoint temperature over a 48-hour period, highlighting heating and cooling zones.
*   **📄 Data Output:** Produces a pandas DataFrame containing the simulation data (Hour, Actual Temperature, Setpoint Temperature, Action).

## 🚀 Getting Started

### Prerequisites

*   Python 3.x
*   Required libraries: NumPy, Matplotlib, Pandas

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
    cd YOUR_REPOSITORY_NAME
    ```
    *(Replace `YOUR_USERNAME` and `YOUR_REPOSITORY_NAME` with your actual GitHub username and repo name)*

2.  **Install dependencies:**
    ```bash
    pip install numpy matplotlib pandas jupyter
    ```
    *(Or, if you create a `requirements.txt` file, use `pip install -r requirements.txt`)*

## 💻 Usage

1.  **Open the Jupyter Notebook:**
    Launch Jupyter Notebook or Jupyter Lab and open the `Control project(2).ipynb` file.
    ```bash
    jupyter notebook "Control project(2).ipynb"
    ```
    *(Alternatively, open it in VS Code with the Python and Jupyter extensions installed).*

2.  **Run the cells:**
    Execute the cells in the notebook sequentially (e.g., using Shift+Enter).

3.  **View the results:**
    The notebook will display:
    *   A plot visualizing the temperature simulation.
    *   The head of the pandas DataFrame showing the first few rows of the simulation data.

## 🛠️ Technology Stack

*   **Python:** Core programming language.
*   **NumPy:** For numerical operations and random number generation.
*   **Matplotlib:** For plotting the simulation results.
*   **Pandas:** For creating and managing the simulation data in a DataFrame.
*   **Jupyter Notebook:** For interactive code execution and visualization.

## ⚙️ Simulation Details

*   **Schedule:** The `get_setpoint()` function defines the desired temperature based on the hour of the day (modulo 24).
*   **Control Logic:**
    *   Heating activates if `setpoint - current_temp > 1`.
    *   Cooling activates if `setpoint - current_temp < -1`.
    *   Otherwise, the system is idle.
*   **Temperature Model:** A simplified model where temperature changes by ±0.8°C per hour when heating/cooling, plus small random fluctuations (`numpy.random.normal`).
*   **Duration:** The simulation runs for 48 hours.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue if you have suggestions or find bugs.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details. *(Make sure you add a LICENSE.md file to your repository)*

## 📧 Contact

Project Link: [[https://github.com/HendElHout/Automatic-Room-Temperature-Scheduler-with-Feedback-Logic.](https://github.com/HendElHout/Automatic-Room-Temperature-Scheduler-with-Feedback-Logic)](https://github.com/HendElHout/Automatic-Room-Temperature-Scheduler-with-Feedback-Logic.)
