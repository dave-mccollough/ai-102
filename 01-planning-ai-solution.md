Once trained, the LLM can take an input (called a prompt) and generate coherent, context-aware output in response.# Planning an Azure AI solution

- Understanding Machine Learning
  - Artifical Intelligence
    - Machine Learning
      - Machine Learning is a part of artifical intelligence
      - Machine learning models are developed with data and algorithms
      - Models can make predections
      - Models can be used to detect fradualent bank transactions
    - Deep Learning
      - Type of machine learning model
      - Models have capability to recognize complex objects - pictures, text and sounds
        - Computer Vision
    - Building a machine learning module
      - Business use case
      - Prepare data
      - Apply appropiate algorithm
      - Build model
      - Evaluation
      - Deploy model
      - Monitor model
  
- Generative AI
  - Generative AI is a type of artificial intelligence that can create new content — such as text, images, music, code, or videos — rather than just analyzing or classifying existing data. It’s called “generative” because it generates outputs that didn’t exist before, often resembling human-created work.

- What are LLMs
  - LLMs, or Large Language Models, are a type of artificial intelligence system that can understand, generate, and reason about human language.
  - They’re the core technology behind tools like ChatGPT, Google Gemini, and Anthropic Claude
  - The model is fed huge amounts of text data and learns statistical relationships between words (for example, “coffee” is often near “cup” or “morning”).
  - Most modern LLMs are built using a type of neural network called a Transformer — introduced by Google in 2017 — which excels at understanding context across long stretches of text.
  - Once trained, the LLM can take an input (called a prompt) and generate coherent, context-aware output in response.
  - LLMs are the language focused part of generative AI

- Multi-modal LLM
  - Multimodal LLMs are large language models that can process and generate more than one type of data, not just text
    - Text
    - Images
    - Audio
    - Video
    - Code
  
  - Azure AI Services
    - Azure AI Vision
      - Allows you to process images
        - Optical Character Recognition
          - Extract text from image
            - Extract printed and handwritten text from photos and documents
        - Image Analysis
          - Extract visual features from images such as objects and faces from images
        - Face
          - Detect, recognize and analyze human faces in images
  
    - Azure AI Language Services
      - Provides natural language processing features
        - Named Entity Recognition
          - Helps identify different entities in text and catagorize them
        - Language Detection
          - Helps evaluate text and detect a wide range of languages
        - Sentiment Analysis
          - Analyzes text and identify positive or negative sentiment
        - Key Phrase Extraction
          - Returns main concepts from unstructed text/data

    - Speech Services
      - Convert speect to text
      - Synthesize text to speech
      - Translate Speech

    - Translator Service
      - Text translation capabilities
        - Translate text from one language to another
        - Create tailored translation models
        - Detect the source text language

    - Azure AI Video Indexer
      - Built on top of existing Azure AI services including Translator, Vision, and Speech
      - Extracts insights based on video and audio content
      - Can be used for deep search, content creation, etc

    - Azure AI Document Intelligence
      - Injest documents and forms 
      - Extract data from injested documents
      - Provides prebuilt models or you can customize your own

    - Azure OpenAI
      - Provides access to OpenAI models
        - Base GPT Models
        - Reasoning Models
        - Image Generation

- AI Safety and Responsibility
  - Privacy and Security
    - All systems should be secure and respect privacy
  - Inclusiveness
    - Empower everyone and engage all people
  - Transparency
    - AI Systems should be understandable
  - Accountability
    - People should be accountable for AI systems