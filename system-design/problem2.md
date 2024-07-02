# Problem 2
You are requested to design an Intelligent Document Processing system. This system allows users to process a wide variety of uploaded documents; it tries to match each document to one of its known templates and then recognizes all related keys and values according to all known keys of that classified template.
The uploaded document has to go through several steps. If it has multiple pages, it should be split into pages, and the process below should be applied to an individual page:
- Standardization
- Creating thumbnails
- Pre-processing (Deskew, Rotate, etc.)
- Classification
- Layout
- OCR
- KV matching
- Post-processing

After the file processing is finalized, the user can retrieve information regarding which document type it is, all keys and values recognized, and they should be able to update any value if it's not accurate, then save the last result.

Design a system for the above requirements, that consists of
- A high-level diagram that demonstrates the overview of the system architecture.
- A thorough explanation for each component.
- Specify protocol between components.
- Database/entity design.
- API design for each component/service if needed.

The services must have high availability and scalability.
