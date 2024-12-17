Description - Developed an AI model that calculates each student’s final score by converting long subjective scanned answer sheets into readable text format using OCR and employing techniques such as BERT and Jaccard similarity to compare student responses with correct answers, minimizing the need for human intervention.

OCR (Optical Character Recognition):
Tools like Tesseract OCR or Google Vision API are employed to convert scanned handwritten or printed answer sheets into machine-readable text. This step is crucial for transforming physical documents into a digital format for further analysis.

Natural Language Processing (NLP):
Advanced models like BERT (Bidirectional Encoder Representations from Transformers) are used to process and understand the semantic meaning of student responses. BERT’s pre-trained language understanding helps in comparing student answers to correct ones by analyzing context and synonyms rather than relying solely on exact word matches.

Text Similarity:
Jaccard Similarity is utilized to compare the overlap between student responses and the correct answers. This metric helps in determining how similar the student’s response is to the expected correct answer by assessing the intersection over the union of unique words or phrases.

Scoring Algorithm:
A custom scoring algorithm, built using Python and libraries like Pandas, calculates the final score based on the degree of match between the student’s answer and the correct answer, applying thresholds for full or partial credit.

Deployment & Automation:
The solution is deployed using Docker for containerization and cloud platforms like AWS or Google Cloud for scalability. This ensures the system can process large volumes of answer sheets efficiently in an automated pipeline.
