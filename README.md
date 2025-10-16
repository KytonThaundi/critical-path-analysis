# Critical Path Method (CPM) Analysis

This repository contains a comprehensive analysis and documentation of a project network using the Critical Path Method (CPM). The documentation is built using MkDocs and provides detailed insights into project scheduling and network analysis.

## Overview

The Critical Path Method (CPM) is a project modeling technique used to determine the longest path of planned activities to the end of the project. This analysis includes:

- Detailed network diagram visualization
- Activity duration calculations
- Early and Late start/finish times
- Critical path identification
- Float (slack) analysis
- Total project duration calculation

## Project Structure

```
docs/
├── images/                    # Diagram and visual assets
├── index.md                  # Home page and introduction
├── problem.md                # Problem statement and requirements
├── network-analysis.md       # Network diagram and path analysis
├── critical-path.md          # Critical path calculations
└── results.md               # Results and conclusions
```

## Key Findings

- **Total Project Duration**: 43 days
- **Critical Path**: A → B → F → G → H → I → J → V
- **Number of Activities**: 22
- **Starting Points**: 3 independent activities (A, K, and T)
- **Convergence Points**: Multiple paths merge at activities H, I, and R

## Documentation Setup

### Prerequisites
- Python 3.x
- MkDocs
- Material theme for MkDocs

### Installation

```bash
# Install MkDocs and the Material theme
pip install mkdocs mkdocs-material

# Clone the repository
git clone https://github.com/KytonThaundi/critical-path-analysis.git
cd critical-path-analysis

# Serve the documentation locally
mkdocs serve
```

### Viewing the Documentation

After running `mkdocs serve`, visit `http://127.0.0.1:8000` in your web browser to view the documentation.

## Project Activities

| Activity | Duration (days) | Preceding Activities |
|----------|----------------|---------------------|
| A | 15 | - |
| B | 5 | A |
| C | 6 | B |
| D | 3 | C |
| E | 5 | B |
| F | 10 | B |
| G | 3 | F |
| H | 2 | G, U |
| I | 1 | D, E, H |
| J | 2 | I |
| K | 10 | - |
| L | 10 | K |
| M | 5 | L, O |
| N | 2 | M, U |
| O | 5 | K |
| P | 6 | O |
| Q | 1 | O |
| R | 1 | N, P, Q |
| S | 2 | R |
| T | 10 | - |
| U | 8 | T |
| V | 5 | J, S |

## Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch
3. Make your improvements
4. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.