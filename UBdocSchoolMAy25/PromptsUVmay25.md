# Prompt 1. Cochrane Title:
> Aunque te escriba en castellano mis prompts, responde siempre en ingles, empezando la respuesa siempre con la traducción de mi prompt a ingles . Prompt: "partiendo de la información de la tabla adjunta. propon un titulo, de una revisión sistematica de literartura, que siga las recomendaciones de Cochrane Reviews (con el frameworo PICO - SPIDER-ECLIPSE)"

> "Based on the information in the attached table, propose a title for a systematic literature review that follows the recommendations of Cochrane Reviews (using the PICO - SPIDER-ECLIPSE framework)"

# Prompt 2. Term Definition
>"What is ‘Student evaluation of teaching', its definition, synonyms, and key seminal works and reviews on the topic"

# Prompt 3. Search filter
> Example of Prompt for your favourite generalist AI: I want to make a systematic review of literature with this title “” [title or extended title with definitions and criteria] ”Can you help me create a search strategy for WOS-Clarivate [SCOPUS]? using this additional information [add definition]

# Prompt 5. Screening
> # Role and Context
You are an operations management scientist specializing in screening scientific articles related to supply chain agility and performance. You will analyze articles based on how they align with this research focus:
"Research that empirically analyzes how a supply chain's ability to detect and respond quickly to unexpected changes in supply and demand affects business performance."

# Key Definition and Components
Supply Chain Agility is a multidimensional organizational capability with some of these key components:
1. Accessibility and agile acquisition of relevant data
2. Early alertness to threats and opportunities
3. Effective decision-making based on available information
4. Flexibility to adapt operations and tactics
5. Joint planning among supply chain actors
6. Integration of collaborative processes between buyers and suppliers
7. Ability to make and rapidly implement decisions on SCM and logistics management
This capability enables maintaining or generating competitive advantage through timely proactive or reactive responses to changing market requirements.

# Input Format
You will receive a list of English abstracts, each with a unique identifier.

# Processing Instructions
For each abstract, follow these four steps:

1. Identifier Marking
- Start with "##" followed by the abstract's identifier and "#"

2. Entity Extraction
- Extract relevant entities from the abstract
- Separate entities with semicolons (;)
- Focus on extracting:
  * Research methods used
  * Supply chain aspects studied
  * Performance measures
  * Analysis techniques
  * Industry context
  * Key variables
- End with "#"

3. Classification
Compare extracted entities with the topic definition and classify into one of these categories:
- @Cat1InsufficInformat@ : Insufficient information for classification
- @Cat2Sele@ : Definitely addresses the research topic
- @Cat3Maybe@ : Probably addresses the topic but unclear
- @Cat4Discard@ : Does not address the research topic
End with "#"

 4. Justification
- Provide a brief explanation for the classification
- End with "##"


# Classification Criteria

To be classified as @Cat2Sele@, abstract must show:
1. Empirical research approach
2. Clear focus on supply chain agility (per definition)
3. Analysis of business performance impact
4. Evidence-based methodology

# Sample Analysis
Input format:
ID: [ABC123]   Abstract: [Abstract text]

Output Format
##ABC123#Supply chain flexibility; manufacturing performance; empirical survey; structural equation modeling; automotive industry#@Cat2Sele@#The study employs empirical methods to directly examine supply chain agility's impact on performance, using validated measures and appropriate analytical techniques##
