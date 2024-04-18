![1,000+ PDFs Either Malicious or Benign (4)](https://github.com/chirag-xcvii/CyberSec-Malware-Detection/assets/146003422/88f8044d-2053-4db6-abd4-3f0eb42bb091)
# VCExplorer-Chatbot

**Introduction and Business Problem**
The venture capital industry presents a formidable challenge for younger professionals due to its complex concepts and terminology. VCExplorerBot aims to simplify venture capital concepts, making them more accessible and comprehensible.

![ChiragBOT-ezgif com-video-to-gif-converter](https://github.com/chirag-xcvii/CyberSec-Malware-Detection/assets/146003422/6e35301a-8114-4088-8bd9-d36c9832a4a3)

*Challenges Addressed:*
- Complexity of Concepts: Venture capital's intricate concepts and deal structures can overwhelm newcomers.
- Lack of Accessible Information: Limited access to easy-to-understand resources hinders the learning process.
- Absence of Interactive Learning Tools: Traditional materials often lack interactivity, posing challenges for effective engagement.

**Key Features**

- *Multi-Agent Perspective:* Choose from different agent perspectives, such as Engineer, Mathematician, Teacher, Investor, and Startup founder, to get explanations tailored to specific contexts.
- *Document-Based Knowledge:* The chatbot's knowledge base is built by extracting information from PDF documents and CSV files, providing accurate and up-to-date information. Initially, the plan was to use Tracxn or Crunchbase API for updated data of funding activity in the startup ecosystem, but due to cost concerns, CSV files are utilized.
- *Conversational Retrieval:* Utilizes a Conversational Retrieval Chain, integrating a ChatOpenAI language model with a document retriever, enabling the chatbot to engage in meaningful conversations and retrieve relevant information from source documents.

**User Instructions**

- Select an agent perspective from the dropdown menu (Engineer, Mathematician, Teacher, Investor, Startup founder).
- Type your question or request in the text input field.
- Click the "Submit" button to receive a response from the chatbot.
- Explore different agent perspectives to see how explanations vary based on the selected role.

**Technical Innovations**

- *Document Loading:* Uses PyPDFLoader for PDF documents and CSVLoader for CSV files, establishing a comprehensive knowledge base.
![Screenshot 2024-04-18 205920](https://github.com/chirag-xcvii/CyberSec-Malware-Detection/assets/146003422/852c2a91-9721-48f5-9a9c-1e62ed62f064)
- *Text Splitting:* Implements RecursiveCharacterTextSplitter to enhance efficiency by breaking down text into manageable chunks.
- *Embeddings and Vectorization:* Utilizes OpenAIEmbeddings to transform textual content into numerical representations, creating a FAISS vector store for efficient similarity searches.
- *Conversational Retrieval Chain:* Integrates ChatOpenAI with a document retriever, allowing the chatbot to engage in conversations, answer questions, and transparently provide source documents.

**Acknowledgments**

- *OpenAI:* Powered by the GPT-3.5 Turbo language model from OpenAI.
- *PyPDFLoader and CSVLoader:* Used for document loading and extraction.
- *FAISS:* Employed for vectorization and efficient similarity searches.
- *Gradio:* The interactive interface is built using Gradio.
