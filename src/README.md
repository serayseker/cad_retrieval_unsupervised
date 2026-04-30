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
