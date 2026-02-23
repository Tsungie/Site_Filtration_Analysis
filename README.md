# EHR Database Extraction & Analysis

## Overview
This tool automates the batch processing of numerous MySQL database backups. 
It systematically restores each database into a Dockerized MySQL instance, extracts specific healthcare datasets (including demographics, ART, HTS, and CBS records),
and compiles the aggregated data into high-performance `.feather` files for rapid data science analysis. It also generates a comprehensive log of the extraction process.

## Prerequisites
Before running this script, ensure you have the following installed and running:
* **Python 3.8+**
* **Docker** (running a MySQL container on port `3307` with no root password).
* **MySQL Command Line Tools** (required for the `subprocess` database restoration).

## Installation

1. **Clone the repository** (if applicable):
   ```bash
   git clone <repository-url>
   cd <repository-folder>
