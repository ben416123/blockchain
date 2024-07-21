# Simple Blockchain Implementation with Flask

This is a basic implementation of a blockchain using Python and Flask. This project was built as part of my effort to understand how blockchains work by following the guide at [Learn Blockchains by Building One](https://hackernoon.com/learn-blockchains-by-building-one-117428612f46).

## Features
- Basic blockchain structure with proof of work
- Simple transaction mechanism
- Flask web server with endpoints to interact with the blockchain

## Endpoints
- `GET /mine`: Mines a new block and rewards the node.
- `POST /transactions/new`: Adds a new transaction to the next mined block.
- `GET /chain`: Returns the full blockchain.

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/blockchain.git
    cd blockchain
    ```

2. **Create and activate a virtual environment:**
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required packages:**
    ```sh
    pip install Flask
    ```

4. **Run the application:**
    ```sh
    python blockchain.py
    ```

The Flask application will start and listen on port 5000.

## Usage

### Mine a New Block
To mine a new block, send a GET request to `/mine`:

```sh
curl http://localhost:5000/mine
```

# Acknowledgments
This project is based on the guide "Learn Blockchains by Building One" by Daniel van Flymen. The guide was instrumental in helping me understand the fundamentals of blockchains by building one from scratch.

# License
This project is open source and available under the MIT License.