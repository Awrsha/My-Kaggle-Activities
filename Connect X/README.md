# ConnectX Agent

## Overview
This repository contains an agent implemented in Python for playing the game ConnectX. The agent utilizes a strategy based on analyzing patterns on the game board to make informed decisions.

## Requirements
- Python 3.x
- Kaggle `gym` library (for running the ConnectX environment)
- Other dependencies as listed in `requirements.txt`

## Getting Started
1. Clone this repository to your local machine.
2. Install the required dependencies by running:
   ```
   pip install -r requirements.txt
   ```
3. Run the agent against itself or another opponent using the provided scripts or integrate it into your ConnectX game environment.

## Usage
- To run the agent against itself:
  ```
  python play_agent.py
  ```
- To train the agent against a built-in opponent:
  ```
  python train_agent.py
  ```
- To integrate the agent into a ConnectX game environment:
  ```python
  import connectx_agent
  
  # Load the agent
  agent = connectx_agent.load_agent("path/to/agent.py")
  
  # Run the game with the agent
  game = connectx_agent.ConnectXGame()
  game.run(agent)
  ```

## File Structure
- `submission.py`: Contains the implementation of the ConnectX agent.
- `play_agent.py`: Script to play the agent against itself.
- `train_agent.py`: Script to train the agent against a built-in opponent.
- `connectx_agent.py`: Helper module for integrating the agent into ConnectX game environments.
- `requirements.txt`: List of Python dependencies.
- `README.md`: This file.

## Contributing
Contributions are welcome! If you find any bugs or have suggestions for improvements, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
