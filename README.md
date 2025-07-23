# Repository zur Bachelorarbeit von Laurenz Brahner

**Titel der Arbeit**  
*Fehlinformationen im KI-gestützten Informationsabruf - eine experimentelle Untersuchung verschiedener RAG-Ansätze*

**Hochschule der Medien Stuttgart - Sommersemester 2025**  
**Studiengang Wirtschaftsinformatik und digitale Medien (WI7)**  
**Erstbetreuer: Prof. Dr. Hendrik Meth**  
**Zweitbetreuer: Prof. Dr. Jan Kirenz**


## Inhalt des Repositories

Dieses Repository enthält den Code für die Bachelorarbeit von Laurenz Brahner (lb184).


## Ordnerstruktur

```
experiment_bachelor_lb184/
|-- antworten_der_systeme_manipuliert_beide_durchgänge/
|    |-------- CSV-Dateien mit den Antworten der im manipulierten Kontext
|-- antworten_der_systeme_originalkontext_beide_durchgänge/
|    |-------- CSV- Dateien mit den Antworten im originalkontext
|-- Datenmanipulation/
|   |-- fragen_und_loesungen/
|        |------- Textdateien mit Fragen und Lösungen zu den artikeln
|   |-- manipulierte_artikel/
|        |------- Textdateien mit den Injizierten Fake News
|   |-- manipulierte_artikel_ohne_markierung/
|        |------- Textdateien mit den Injizierten Fake News ohne Markierung (Kontext für RAG)
|   |-- originalartikel/
|        |------- Textdateien mit den Originalartikel
    |-- Notebooks zur Artikelverarbeiung und manipulation sowie Excel-Datei mit den Artikeln, Links und Abrufdatum
|-- evaluation/
│   |-- llm_bewertungen_manipulierter_kontext_beide_durchgänge/
|        |------- CSVs mit den Bewertungen im originalkontext
|   |-- llm_bewertung_originalkontext_beide_durchgänge/
|        |------- CSVs mit den Bewertungen im manipulierten Kontext
|   |-- manuelle_evaluation_csv/
|        |------- CSVs mit der Stichrpobe, der Bewerteten Stichprobe und der Übereinstimmung zwischen Autor und LLM
|   |-- notebooks/
|        |------- notebooks zur deskriptiven und statistischen Auswertung, der Evaluation und 
|   |-- schaubilder/
|        |------- Erstelle Schaubilder als png
|-- prompts/
|   |-- Alle verwendeten Prompts als Textdateien
|-- RAG_Systeme/
|   |-- Notebooks mit der Implementierung der RAG-Systemen
 ```

## Kurzanleitung und Requirements
1. Virtuelles Environment erstellen
   
   `python -m venv <name_der_umgebung>`

2. Requirements installieren
   `pip install -r requiremnts.txt`

3. `.env` Datei erstellen mit
   
   `OPEN_AI_API_KEY = <key einfügen>
   NEO4J_URI =  <URI zur instanz>
   NEO4J_USERNAME = <Username>
   NEO4J_PASSWORD =  <Passwort>`


## Quellen 

```
Langchain. (o. D.). LangChain Documentation: Introduction. LangChain. Abgerufen am 14. Mai 2025, von https://python.langchain.com/docs/introduction/

LangChain. (o. D.-a). ChatOpenAI. Abgerufen am 7. Juni 2025, von https://python.langchain.com/api_reference/openai/chat_models/langchain_openai.chat_models.base.ChatOpenAI.html

LangChain. (o. D.-b). ChatPromptTemplate. Abgerufen am 5. Mai 2025, von https://python.langchain.com/api_reference/core/prompts/langchain_core.prompts.chat.ChatPromptTemplate.html

LangChain. (o. D.-c). InMemoryVectorStore. Abgerufen am 6. Juni 2025, von https://python.langchain.com/api_reference/core/vectorstores/langchain_core.vectorstores.in_memory.InMemoryVectorStore.html

LangChain. (o. D.-d). LangChain Expression Language (LCEL). Abgerufen am 5. Juni 2025, von https://python.langchain.com/docs/concepts/lcel/

LangChain. (o. D.-e). Neo4jGraph. Abgerufen am 18. Mai 2025, von https://python.langchain.com/api_reference/neo4j/graphs/langchain_neo4j.graphs.neo4j_graph.Neo4jGraph.html


LangChain. (o. D.-f). OpenAIEmbeddings. https://python.langchain.com/api_reference/openai/embeddings/langchain_openai.embeddings.base.OpenAIEmbeddings.html

LangChain. (o. D.-g). RecursiveCharacterTextSplitter. Abgerufen am 18. Mai 2025, von https://python.langchain.com/api_reference/text_splitters/character/langchain_text_splitters.character.RecursiveCharacterTextSplitter.html

LangChain. (o. D.-h). RunnablePassthrough. https://python.langchain.com/api_reference/core/runnables/langchain_core.runnables.passthrough.RunnablePassthrough.html

LangChain. (o. D.-i). StrOutputParser. https://python.langchain.com/api_reference/core/output_parsers/langchain_core.output_parsers.string.StrOutputParser.html

LangChain. (o. D.-j). TextLoader. Langchain. Abgerufen am 20. Mai 2025, von https://python.langchain.com/api_reference/community/document_loaders/langchain_community.document_loaders.text.TextLoader.html


Neo4j. (o. D.). Neo4j Aura Documentation. Abgerufen am 26. Mai 2025, von https://neo4j.com/docs/aura/

Neo4j. (2025). Neo4j LLM Knowledge Graph Builder. https://neo4j.com/labs/genai-ecosystem/llm-graph-builder/

OpenAI. (2022). Text-embedding-ada-002. Abgerufen am 6. Juni 2025, von https://platform.openai.com/docs/models/text-embedding-ada-002

OpenAI. (2024). Gpt4-o. Abgerufen am 6. Juni 2025, von https://platform.openai.com/docs/models/gpt-4o

Plotly. (o. D.). Plotly Express in Python. Abgerufen am 16. Juli 2025, von https://plotly.com/python/plotly-express/

Pandas. (2025, 7. Juli). Pandas Documentation. Abgerufen am 11. Juli 2025, von https://pandas.pydata.org/docs/

Python. (2023). Python 3.12.0 Documentation. Abgerufen am 5. Mai 2025, von https://docs.python.org/release/3.12.0/

Jupyter. (o. D.). Project Jupyter Documentation. Abgerufen am 12. Mai 2025, von https://docs.jupyter.org/en/latest/

SciPy. (o. D.). chi2_contingency. Abgerufen am 1. Juli 2025, von https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.chi2_contingency.html

sh-how. (2024). enhancing_rag_with_graph.ipynb. GitHub. Abgerufen am 7. Mai 2025, von https://github.com/Coding-Crashkurse/GraphRAG-with-Llama-3.1/blob/main/enhancing_rag_with_graph.ipynb

```
