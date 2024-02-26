# KFC Drive-Thru Ordering automation RAG

Akshay Shastri
akshay.shastri@student-cs.fr

This repository contains code for a KFC drive-thru ordering automation RAG. The system leverages advanced language models to provide an interactive ordering experience similar to interacting with a human attendant at a drive-thru.

## Why Case 1


Familiarity: The coding challenge was time-limited, and I had previously created a similar RAG (Retrieval Augmented Generation) model out of curiosity. Given my prior experience, I anticipated that it would be easier to complete the task quickly as I only needed to adapt some code from PDF to JSON format.


## Models Used

The system utilizes two Hugging Face models:

1. **Llama-2-7b-chat-hf**: This model is trained on conversational data and serves as the primary language model for generating responses to customer queries.
2. **MiniLM-L6-v2**: This model is used for embeddings to represent document chunks, aiding in efficient retrieval of information from the menu.

## Functionality

- The system is designed to handle customer queries and provide accurate responses regarding menu items, availability, pricing, and nutritional information.
- It incorporates a system prompt guiding the response behavior of the language model to ensure helpful and accurate responses similar to a human attendant.
- A query wrapper prompt is employed to format customer queries for the language model.
- Menu data is loaded from a JSON file, and an index is created to facilitate quick and efficient querying of menu items.
- The system provides an example usage scenario where a customer query is processed, and the system responds with information regarding the availability of a menu item (e.g., cola).

## Usage

To use the KFC drive-thru ordering automation service:

1. Set up environment variables for model access.
2. Create the tokenizer and model instances.
3. Define system and query wrapper prompts for guiding the language model behavior.
4. Set up embeddings for document chunk representation.
5. Load menu data from a JSON file and create an index.
6. Use the index query engine to process customer queries and generate responses.


## Further Improvements

1. **Scalability and Deployment**: Design the system with scalability in mind to accommodate varying levels of demand, especially during peak hours or promotions. Utilize cloud-based infrastructure and containerization technologies such as Docker and Kubernetes to enable easy scaling and deployment across multiple servers or regions. Implement load balancing and auto-scaling mechanisms to dynamically allocate resources based on traffic patterns, ensuring optimal performance and reliability. Additionally, automate deployment processes using continuous integration and continuous deployment (CI/CD) pipelines to streamline updates and maintenance tasks, reducing downtime and ensuring seamless operation of the ordering system.
2. **Multi-turn Conversation Handling**: Enhance the system to handle multi-turn conversations, where the system can maintain context across multiple customer interactions, providing a more seamless and human-like experience.

 3. **Error Handling and Recovery**: Implement robust error handling mechanisms to gracefully handle unexpected inputs or errors during the interaction. Additionally, incorporate recovery strategies to handle misunderstandings or incomplete queries effectively.

 4. **Dynamic Menu Updates**: Enable the system to dynamically update the menu based on real-time changes, such as new menu items, price adjustments, or item availability. This ensures that the information provided to customers is always up-to-date and accurate.

 5. **Personalization and Recommendations** : Implement personalization features to tailor responses based on customer preferences and past interactions. Additionally, incorporate recommendation systems to suggest menu items based on customer preferences, dietary restrictions, or popular choices.

6. **Performance Optimization**: Optimize the performance of the system, including reducing response times, minimizing resource usage, and optimizing memory footprint, to ensure efficient operation, especially during peak usage periods.
7. **Feedback Mechanism**: Implement a feedback mechanism to collect customer feedback on the ordering experience and use it to continuously improve the system's performance, accuracy, and user satisfaction.
