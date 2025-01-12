# Pathfinder — Graph Shortest-Path Visualiser

An interactive desktop tool for visualising Dijkstra's and BFS shortest-path algorithms on weighted graphs, built with Python and Tkinter.

## Features

- Build graphs interactively — add nodes and weighted edges on a canvas
- Choose between **Dijkstra's algorithm** (weighted graphs) and **BFS** (unweighted graphs)
- Step-by-step animation mode
- Path highlighting with total cost display
- Save and load graphs as JSON files
- Preset example graphs for quick demos
- Disconnected graph detection with a user-friendly message

## Stack

| Layer | Technology |
|---|---|
| Language | Python 3.11+ |
| GUI | Tkinter |
| Dependencies | Standard library only |

## Getting Started

```bash
git clone https://github.com/starpearl03/pathfinder-gui
cd pathfinder-gui
python src/main.py
```

## Usage

1. Click the canvas to add nodes
2. Select two nodes and enter a weight to add an edge
3. Choose source and target nodes from the dropdowns
4. Select algorithm (Dijkstra / BFS) and click **Find Path**
5. Use **Step** for animation or **Run** to see the full result at once

## Project Structure

```
src/
├── algorithm.py   # Dijkstra and BFS implementations
├── canvas.py      # Drawing helpers (nodes, edges, path highlight)
├── graph.py       # Weighted adjacency-list graph data structure
├── gui.py         # Main application window and event handling
├── io.py          # JSON graph save / load
└── state.py       # Application state dataclass
tests/
├── test_algorithm.py
└── test_graph.py
```

## Configuration

Copy `.env.example` and adjust display settings:

```bash
cp .env.example .env
```

| Variable | Default | Description |
|---|---|---|
| `APP_WIDTH` | 800 | Canvas width in pixels |
| `APP_HEIGHT` | 600 | Canvas height in pixels |
| `DEFAULT_GRAPH` | none | Path to a graph JSON to load on startup |

## Author

Felistas V. Charuka · [github.com/starpearl03](https://github.com/starpearl03)
