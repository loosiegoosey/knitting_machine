# Knitting Machine Readme

## Project Title
Knitting Machine Tools

## Overview
This project provides a set of tools designed to assist with the operation and management of Brother knitting machines. The tools allow users to dump patterns, emulate PDD, and process images for knitting patterns.

## Features
- **Brother Knitting Machine Interface**:
  Interface for communicating with Brother knitting machines.
  
- **Pattern Dumping**:
  Tools for extracting knitting patterns from the machines.
  
- **PDD Emulation**:
  Emulate PDD (Pattern Design Database) to manage patterns more efficiently.
  
- **Image Processing**:
  Process images to create knitting patterns based on graphical input.

## Installation Instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Yuriy/knitting_machine.git
   cd knitting_machine
   ```

2. **Install dependencies**:
   The project requires Python and the PIL (Python Imaging Library). Install PIL using pip:
   ```bash
   pip install pillow
   ```
   
3. **Make scripts executable** (Optional for Unix-like systems):
   ```bash
   chmod +x brother.py dumppattern.py PDDemu-debug.py PDDemulate-1.0.py process_image.py
   ```

4. **Run the scripts**:
   Ensure Python environment is set up correctly.
   ```bash
   ./brother.py
   ./dumppattern.py
   ./PDDemu-debug.py
   ./PDDemulate-1.0.py
   ./process_image.py
   ```

## Usage Examples
### Dumping patterns:
To dump patterns from the knitting machine, run:
```command line
python dumppattern.py
```

### Emulating PDD:
For PDD emulation, use:
```command line
python PDDemulate-1.0.py
```

### Processing an image:
To create a knitting pattern from an image, place your image in the same directory and run:
```python
python process_image.py image_file.png
```
Example Output for an image processing:
```python
width: 100
height: 50
* * * * *       ...
```

## Code Summary
The project is composed of the following key scripts:
- **brother.py**: Interface script for Brother knitting machine.
- **dumppattern.py**: Script to dump patterns from the knitting machine.
- **PDDemu-debug.py**: Debugging tool for PDD emulation.
- **PDDemulate-1.0.py**: Main script for PDD emulation.
- **process_image.py**: Handles image processing for knitting patterns. Uses Python Imaging Library to read an image and convert it to a knitting pattern.

## Contributing Guidelines
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

Please ensure that your contributions follow the coding standards and include appropriate documentation and test cases.

## License
This project is licensed under the GNU General Public License - see the [LICENSE](LICENSE) file for details.