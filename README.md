
# DFSM Simulator

## Overview
The DFSM Simulator is an interactive tool designed to help users understand and visualize Deterministic Finite State Machines (DFSM). This project allows users to define a DFSM by specifying states, input symbols, transitions, start states, and accepting states. The simulator validates input strings step by step, determining whether each string is accepted or rejected according to the DFSM's transition rules.

A dynamic graphical representation of the DFSM is provided, where users can visualize the transition diagram. The diagram highlights the movement between states, including start, accepting, and current states, to enhance the understanding of how the automaton operates.

## Features
- **Define DFSM States**: Specify the number of states, including start and accepting states.
- **Create Transitions**: Define transitions between states based on input symbols.
- **Input String Validation**: Input strings can be validated step-by-step against the DFSM.
- **Interactive Graphical Representation**: Visualize the DFSM as an interactive transition diagram with labeled edges and highlighted states.
- **User-friendly Interface**: Simple input fields for specifying states, transitions, and input strings, with easy-to-follow graphical outputs.

## Requirements
- Python 3.x
- `tkinter` for the GUI
- `graphviz` for generating state diagrams
- `Pillow` for image handling

## Installation
1. Clone the repository or download the project files to your local machine.
2. Install the required libraries:
   ```bash
   pip install tkinter graphviz pillow
   ```
3. Ensure that Graphviz is installed on your system. You can download it from [Graphviz official site](https://graphviz.gitlab.io/download/).

## Usage
1. Launch the simulator by running the `dfsm_simulator.py` script.
   ```bash
   python dfsm_simulator.py
   ```
2. Enter the following inputs:
   - **States**: A comma-separated list of states (e.g., `q0,q1,q2`).
   - **Alphabet**: A comma-separated list of symbols in the alphabet (e.g., `0,1`).
   - **Start State**: The state where the machine starts (e.g., `q0`).
   - **Accepting States**: A comma-separated list of accepting states (e.g., `q1`).
   - **Transitions**: A semicolon-separated list of transitions in the format `state,symbol,next_state` (e.g., `q0,0,q1;q1,1,q2`).
   - **Input String**: The string you want to test (e.g., `011`).
3. Click "Convert NFA to DFA" to simulate the process and see the resulting DFA diagram.

## Example
Input:
- **States**: `q0,q1,q2`
- **Alphabet**: `0,1`
- **Start State**: `q0`
- **Accepting States**: `q2`
- **Transitions**: `q0,0,q1;q1,1,q2;q0,1,q0;q1,0,q0`
- **Input String**: `011`

Output: The program will generate a DFA diagram, and it will validate the string `011`, showing whether it is accepted or rejected based on the DFSM.

## Contributing
Feel free to fork this project and submit pull requests for improvements or fixes. If you have any suggestions or issues, please open an issue in the GitHub repository.

## License
This project is open-source and available under the [MIT License](LICENSE).

---
