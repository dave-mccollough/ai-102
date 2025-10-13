# Implement Generative AI Solutions

## Azure AI Foundry

- Unified platform that streamlines the development and deployment of AI based applications
- Contains a variety of models (including OpenAI models)
- Playground functionality that allows you to experiment with tools
- Two types of projects you can create in Foundry
  - Foundry Project
    - Simple setup with access to models from OpenAI, Meta, etc
  - Hub Based Projects
    - Provides ability to use open-source models, prompt flows, context understanding

- Models
  - Has a large catalog of models from Microsoft or other vendors (model catalog)
  - You can perform a comparison of different models as well as a side by side evaluation of each model
  - After choosing the model you can deploy the model

- Deploying the model
  - Deployment type depends on data residency needs, call volumne, and capacity
  - Different types of deployment types in Azure AI Foundry
    - Standard
    - Provisioned
      - Use provisioned SKU if you need lower latency 
  - Global Deployment
    - Uses Azure global infrastructure
    - Traffic gets routed to the data center with the best availability
    - Prompt and responses may be processed in any geographical area based on the deployment of the Foundry resource
  - Data zone deployment
    - Request is rounted to the data center withing the Microsoft defined datazone with the availability for each request
    - Request processing is kept within the Microsoft data zone
  - Azure AI Foundry is a unified platform for developing, customizing, and managing AI applications and agents. It provides tools and infrastructure for the entire AI development lifecycle, from concept to deployment, and includes access to a wide catalog of models from partners like OpenAI, Hugging Face, and Meta. Key features include secure data integration, model customization, and enterprise-grade governance with features like tracing, monitoring, and evaluations. 

- Model Parameters
  - Settings that can be tweaked to sway the LLM responses
  - Here are a few parameters 
    - Temperature
      - Controls the randomness of the AI models output
      - Settings vary between 0 and 1
        - 0 setting will make the model give more predictable and consistent results
        - 1 setting will make the model more creative in it's responses.
          - Responses will be more varied and diverse
    - Top P
      - Alternative to temperature setting
      - The model takes Top P into consideration when it considers which token to choose next
      - Example
        - If Top P value is 0.1, the model will only consider the top 10%
      - Best practice is to tweak either the Temperature or Top P, but not both at the same time

- Fine Tuning Models
  - Training existing LLMs on your own data set
  - Useful if you need to model to perform specific tasks
  - Reduces overhead for prompt engineering
  - Ensure model aligns with style and tone
  - Output can be formatted the way you want
  - Leads to overall efficiency of the model
  
  - Supervised Fine-Tuning
    - Provide the model custom data
    - Improves the accuray of the model
    - Good if you already have labeled data
  - Reinforcement Fine-Tuning
    - Iterative feedback loop
      - Complex scenarios
      - Model improves through feedback
      - Improve reasoning of the model
  - Direct Preference Optimization
    - Lighter and faster technique for fine tuning models
      - Model weights adjusted
      - Based on human preferences
  
- Tuning process
  - Training and evaluation data
    - Needs to be formatted as JSON lines (JSONL) document
    - Conversational format
  - Choose the model
    - Choose the model you want to fine tune
  - Choose the training method
    - Supervised
    - Direct Preference Optimizaton
    - Reinforcement Fine Tuning
  - Choose training type
    - Standard
      - Occurs in OpenAI's resource region
    - Global
      - Most affordable
      - Does not offer data residency
  - Deploy the model
    - Deploy fine tuned model
  
- Retrival Augmented Generation
  - Augmenting existing LLMs with data that is relevant to your organization
  - Responses should be factually relevant
  - When prompted, the LLM will return data based on it's own knowledge and augmented data
