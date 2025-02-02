#Misinformation Detection System(Truth finder)

This project is a misinformation detection system that utilizes a BERT-based model (SBERT and BERT uncase) along with Google API to verify the credibility of news articles. It provides a user-friendly interface via Gradio to allow users to check the authenticity of news.

Installation & Setup

1. Clone the Repository & Download Data

    First, download the dataset and project files from the GitHub repository:
    
    git clone <your-github-repo-link>
    cd <your-repo-folder>

2. Install Dependencies

    Ensure you have Python installed (preferably 3.8+). Then, install the required dependencies:
    
    pip install -r requirements.txt

3. Set Up API Key & Configuration

    Before running the model, you need to provide your own Google API Key and password.
    
    Open the notebook file (misinformation_detection.ipynb).
    
    Locate the section where the API key is required.
    
    Replace YOUR_GOOGLE_API_KEY_HERE and YOUR_PASSWORD_HERE with your actual credentials.

4. Modify Trusted Sources

    The system verifies news credibility based on a predefined list of trusted news sources. Modify the websites list in the code according to the type of news you want to analyze (e.g., general news, sports, finance, politics, etc.).
    
    Example modification in trusted_sources:
    
    TRUSTED_SOURCES = [
        "bbc.com", "reuters.com", "nytimes.com", "thehindu.com", "ndtv.com"
    ]

Running the Model

1. Open and Run the Jupyter Notebook

    Launch Jupyter Notebook and open misinformation_detection.ipynb:
    
    jupyter notebook
    
    Then run all the cells in order.

2. Click on the Gradio Link

    Once the notebook runs successfully, a Gradio interface link will appear. Click on it to open the web UI in your browser.

3. Enter the News for Verification

    In the Gradio interface:
    
    Type or paste the news headline or content.
    
    Click Check to get the misinformation detection result.

#Dataset: Taken from kaggle fake news_detection repositery

