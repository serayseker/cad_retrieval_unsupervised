# Unsupervised clustering of industrial CAD models for design retrieval from database <img width="300" height="21" alt="image" src="https://github.com/user-attachments/assets/8e4bee28-a08e-4fad-9970-6b8254320b15" />



# Project Structure

This repository is organized to support the development of an unsupervised pipeline for CAD model retrieval. The structure separates data handling, core implementation, experimentation, and documentation to ensure clarity and scalability.

<img width="695" height="400" alt="image" src="https://github.com/user-attachments/assets/7377eeb1-3f12-46e2-b87c-cac68cd4e297" />


---

## Root Directory

Main project directory containing all source code, data references, experiments, and documentation.

---

## Data

- **raw/**  
  Contains original CAD datasets (e.g., STEP files) as obtained from external sources.  
  These files should remain unchanged.

- **processed/**  
  Stores transformed data such as graph representations derived from CAD models.  
  Includes intermediate outputs used for training and evaluation.

- **subsets/**  
  Smaller or filtered portions of the dataset used for debugging, rapid prototyping, or controlled experiments.

---

## Source Code

- **cad_io/**  
  Handles input/output operations for CAD data.  
  Includes parsing of STEP files (e.g., via PythonOCC) and basic geometry extraction.

- **graph_conversion/**  
  Converts CAD representations (e.g., B-Rep) into graph structures.  
  Defines nodes (faces, edges, vertices) and their relationships.

- **models/**  
  Contains implementations of machine learning models, primarily Graph Neural Networks (GNNs) or embedding models.

- **unsupervised/**  
  Implements unsupervised learning approaches such as contrastive learning, clustering, or embedding-based retrieval.

- **utils/**  
  Utility functions shared across modules (e.g., logging, visualization, helper functions).

---

## Experiments

- **configs/**  
  Configuration files defining experiment parameters (e.g., model settings, training hyperparameters).

- **results/**  
  Stores outputs from experiments such as trained embeddings, metrics, and logs.

- **analysis/**  
  Contains scripts and notebooks for evaluating results, performing ablation studies, and generating plots.

---

## Interface

Provides a lightweight user interface for:
- Uploading a CAD model
- Retrieving similar models from the database

This can be implemented as a simple script, web app, or minimal GUI.

---

## Documentation

Contains:
- Literature review
- Methodology notes
- Project reports
- Diagrams and design decisions

---

## Other Files

- **README.md**  
  Overview of the project, setup instructions, and structure (this file).

- **requirements.txt**  
  List of Python dependencies required to run the project.

---

## Notes

- Each module is designed to be modular and independently testable.
- The structure supports iterative experimentation and extension over two semesters.

<img width="1276" height="717" alt="image" src="https://github.com/user-attachments/assets/0037ba66-19c0-416d-901f-3a67c9519e24" />

