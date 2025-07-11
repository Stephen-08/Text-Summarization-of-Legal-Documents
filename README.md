# Text Summarization of Legal Documents using GNN and T5

Text summarization is a crucial task in natural language processing (NLP) that aims to reduce large, complex documents into concise, informative summaries. This is especially important in the legal domain, where the volume and complexity of documents such as case law, contracts, and court rulings require efficient methods for extraction and condensation. Legal documents often contain dense language and intricate details, making traditional summarization approaches challenging. Text summarization methods generally fall into two categories: extractive and abstractive.

Extractive summarization involves selecting key sentences or segments directly from the original document to form a summary.

Abstractive summarization generates entirely new sentences that convey the core meaning of the document, rephrasing and condensing the content.

Legal summarization has unique challenges, given the necessity for accuracy, precision, and clarity. This project addresses these challenges by using a hybrid approach that combines Graph Neural Networks (GNNs) for extractive summarization and T5 (Text-to-Text Transfer Transformer) for abstractive summarization. The absence of a dataset with labeled summaries or ground truth makes supervised learning approaches impractical, so this project leverages unsupervised learning for the GNN component.
Key Components of the Project: Graph Neural Networks (GNNs):

Used for extractive summarization.

Capture the relationships between sentences in a document by modeling the text as a graph, where sentences are nodes and the relationships between them are edges.

Identify key sentences based on their importance and relevance, preserving the critical content of the document without the need for labeled training data.

T5 (Text-to-Text Transfer Transformer):

Used for abstractive summarization.

Generates novel summaries by rephrasing the original text while maintaining the meaning and legal context.

Fine-tuned to specifically handle legal documents, ensuring that the generated summaries are contextually relevant and accurate.

Challenges and Solutions: Lack of Labeled Data: Legal text datasets with ground truth summaries are scarce, making supervised approaches difficult. The solution lies in using unsupervised learning for the GNN, where it learns to identify important sentences based on document structure and sentence relationships.

Complexity of Legal Text: Legal language often contains nuances that are essential for understanding. The combination of GNNs and T5 allows the model to identify salient points while also generating summaries that are both accurate and easy to read.

Project Objectives: Develop a model capable of producing high-quality summaries of legal documents that preserve the important legal details and concepts.

Use unsupervised learning to enable extractive summarization without requiring a labeled dataset.

Combine extractive and abstractive summarization to generate summaries that are both precise (through extraction) and fluent (through generation).

Provide a valuable tool for legal professionals, enabling them to quickly understand key points from lengthy, complex documents.

By integrating unsupervised extractive summarization using GNNs with abstractive summarization via T5, this project aims to create a robust, efficient solution for legal document summarization that enhances both the quality and readability of legal texts. The model will assist legal professionals in improving their workflow, facilitating quicker decision-making, and reducing the time spent on manual document analysis.