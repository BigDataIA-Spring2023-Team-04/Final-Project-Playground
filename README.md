# AIssue Flow :zap:

## Abstract :memo: 

## Project Goals

1. Scrape issue-related data from various GitHub repositories using the GitHub API and store it in a Snowflake database along with associated metadata.
2. Use the BERT model to convert issue bodies into vector embeddings and store them in a Milvus database for efficient similarity search.
3. Develop two main functions, Git Magnet and Git Cognizant, to make the project more user-friendly.
4. Use the ChatGPT model to summarize issues and leverage Milvus to find similar issues for the selected issue.
5. If no similar issues are found, provide assistance to the user through the GPT Intelligent Chatbot to find potential solutions to the issue.

## Use case

The use case for this project could be to help software developers and teams better manage their projects on GitHub. By using the GitHub API to scrape issue-related data, storing it in a database, and leveraging advanced NLP and vector similarity algorithms, developers can more easily search for and find relevant issues, as well as summarize them for quicker understanding. This can lead to faster issue resolution and more efficient project management overall.

## Data Source

The data source for this project is the GitHub API, which provides access to all the issue-related data for public repositories. 

## Process Outline

1. Data Collection: Use GitHub API to extract issue-related data from various repositories and store it in a Snowflake database.
2. Data Preprocessing: Clean and preprocess the collected data to make it suitable for analysis.
3. Feature Extraction: Use the BERT model to extract vector embeddings from the issue body text.
4. Data Validation: Use Great Expectations to validate the collected data and ensure it meets the expected format and values.
5. Vector Embedding: Use the BERT model to convert issue bodies into vector embeddings and store them in a Milvus database.
6. Similarity Search: Use Milvus to search for similar issues based on the generated vector embeddings.
7. User Interface: Build a web application using Streamlit to provide an intuitive interface for users to search and explore the collected issue data and its embeddings.
8. Testing: Use pytest for unit testing to ensure the functionality of the application and its components.
9. Deployment: Host the application in cloud and deploy it using Airflow and a GCP instance.

## Requirements

fastapi==0.92.0
passlib==1.7.4
pydantic==1.10.4
python-dotenv==1.0.0
python-jose==3.3.0
snowflake-connector-python==3.0.2
snowflake-sqlalchemy==1.4.7
:open_file_folder: SQLAlchemy==1.4.47
gunicorn==20.1.0
uvicorn==0.20.0
python-multipart
🔢 numpy==1.23.5
openai==0.27.0
pymilvus==2.2.6
transformers==4.27.4
🖼streamlit==1.18.1








