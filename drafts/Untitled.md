**Technology Selection Framework Questions:**

1. **Approved Platforms/Vendors:** Beyond what you mentioned (AWS Bedrock, Azure OpenAI, Qdrant, Power Automate, Copilot Studio, MS Foundry), are there any other pre-approved or restricted platforms I should include? Any explicit "do not use" vendors?
    we also have Automation Anywhere for RPA as approved vendor.
    
2. **Build vs Buy Preference:** Does Bank ABC have a general preference for build vs buy, or is this purely use-case driven?
	we have SAAS applications, where. AI capabilities might be embedded within the solution by the SAAS provider, also we have Corporate Banking portal and the ila Bank app which is developed in house.
    
3. **Open Source Policy:** What's the stance on open-source models (e.g., Llama, Mistral) - allowed, restricted, or prohibited?
4. we prefer to keep the models limited to Azure OpenAI and AWS Bedrock models, Titan and possibly pivately hosted models (Llama Mistral). as of now we do not host our own models yet,
    

**Development Standards Questions:**

4. **Existing Standards:** Do you have existing software development standards from IT that we need to align with or reference (e.g., coding standards, CI/CD, security scanning)?
   Yes, we have. you can reference to same. 
    
5. **MLOps Tooling:** What's your current/planned MLOps stack - MLflow, Weights & Biases, SageMaker Experiments, or something else?
     yes, MLflow and sagemaker
    
6. **Automation Development:** For RPA/Workflow, is UiPath in use or planned, or is it purely Microsoft Power Platform?
	Automation Anywhere and Microsoft Power Platform.
    

**Validation & Security Questions:**

7. **Independent Validation:** Since Model Risk function is being built, should validation standards assume self-validation initially with a path to independent validation?
    yes, please.
    
8. **Security Scanning:** Any specific security tools already in use (SAST, DAST, container scanning) that should be referenced?
Yes, just reference to security scanning; without mentioning any tools. its a seperarte document.