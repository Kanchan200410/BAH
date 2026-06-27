# Google Earth Engine Python Setup

This repository provides instructions and starter code for setting up and working with the official **Google Earth Engine (GEE) Python API** and interactive mapping tools.

## Prerequisites

Before using Earth Engine, you must have a registered Google Earth Engine account. If you do not have one, sign up at [://google.com](https://://google.com/).

## Installation

Install the official Earth Engine API via `pip`. It is also highly recommended to install `geemap` for interactive data visualization.

```bash
# Install the core Earth Engine API
pip install earthengine-api

# Install interactive mapping support (Recommended for Jupyter/Colab)
pip install geemap
```

### Upgrade Existing Installation
To update an existing installation to the latest version, run:
```bash
pip install earthengine-api --upgrade
```

## Authentication and Initialization

You must authenticate your machine and link it to an active Google Cloud Project before running any scripts. 

Run the following Python code to initiate the setup:

```python
import ee
import geemap

# 1. Trigger the browser authentication flow
ee.Authenticate()

# 2. Initialize the library with your Google Cloud Project ID
ee.Initialize(project='your-cloud-project-id')
```
*Note: `ee.Authenticate()` will open a web browser asking you to sign in with your registered Google account.*

## License
This project is open-source and available under the MIT License.
