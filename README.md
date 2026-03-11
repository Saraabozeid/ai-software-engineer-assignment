AI Software Engineer Assignment (Python)
This repository contains a Python-based HTTP client with OAuth2 token management. It has been updated to fix a logic bug, include pinned dependencies, and support containerized execution via Docker.
## Features
* OAuth2 Token Refresh: Automatically handles token refreshes when tokens are missing, expired, or provided as raw dictionaries.
* Docker Integration: Fully containerized environment for consistent testing.
* Dependency Management: Pinned versions in requirements.txt for reproducibility.
## How to Run the Project
1. Local Environment (On your PC)
To run the tests on your local machine, follow these steps:
1. Install dependencies:
pip install -r requirements.txt

2. Run the test suite:
pytest -v

2. Docker Environment
To build and run the tests in a clean, isolated container:
   1. Build the Docker image:
docker build -t ai-assignment .

   2. Run the tests in the container:
docker run ai-assignment
## Project Structure
      * app/: Core logic (http_client.py and tokens.py).
      * tests/: Project test suite.
      * Dockerfile: Instructions for building the Docker environment.
      * requirements.txt: List of pinned dependencies.
      * Explanation.md: Breakdown of the bug fix and technical reasoning.
