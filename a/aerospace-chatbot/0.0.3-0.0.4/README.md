# Comparing `tmp/aerospace_chatbot-0.0.3.tar.gz` & `tmp/aerospace_chatbot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerospace_chatbot-0.0.3.tar", max compression
+gzip compressed data, was "aerospace_chatbot-0.0.4.tar", max compression
```

## Comparing `aerospace_chatbot-0.0.3.tar` & `aerospace_chatbot-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-11 05:19:38.306973 aerospace_chatbot-0.0.3/LICENSE
--rw-r--r--   0        0        0      506 2024-04-12 00:17:05.632959 aerospace_chatbot-0.0.3/README.md
--rw-r--r--   0        0        0     1306 2024-04-12 00:33:11.560988 aerospace_chatbot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 15:24:34.392942 aerospace_chatbot-0.0.3/src/aerospace_chatbot/__init__.py
--rw-r--r--   0        0        0    36171 2024-04-11 16:01:25.420710 aerospace_chatbot-0.0.3/src/aerospace_chatbot/admin.py
--rw-r--r--   0        0        0    39103 2024-04-12 00:30:22.434117 aerospace_chatbot-0.0.3/src/aerospace_chatbot/data_processing.py
--rw-r--r--   0        0        0      919 2024-03-31 15:24:34.393743 aerospace_chatbot-0.0.3/src/aerospace_chatbot/prompts.py
--rw-r--r--   0        0        0    14656 2024-04-11 05:19:39.989659 aerospace_chatbot-0.0.3/src/aerospace_chatbot/queries.py
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 aerospace_chatbot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 05:19:38.306973 aerospace_chatbot-0.0.4/LICENSE
+-rw-r--r--   0        0        0      506 2024-04-14 01:32:23.236876 aerospace_chatbot-0.0.4/README.md
+-rw-r--r--   0        0        0     1306 2024-04-14 01:37:28.813667 aerospace_chatbot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 15:24:34.392942 aerospace_chatbot-0.0.4/src/aerospace_chatbot/__init__.py
+-rw-r--r--   0        0        0    38187 2024-04-14 01:32:23.239705 aerospace_chatbot-0.0.4/src/aerospace_chatbot/admin.py
+-rw-r--r--   0        0        0    39957 2024-04-14 01:32:23.240643 aerospace_chatbot-0.0.4/src/aerospace_chatbot/data_processing.py
+-rw-r--r--   0        0        0      919 2024-03-31 15:24:34.393743 aerospace_chatbot-0.0.4/src/aerospace_chatbot/prompts.py
+-rw-r--r--   0        0        0    14875 2024-04-14 01:32:23.241786 aerospace_chatbot-0.0.4/src/aerospace_chatbot/queries.py
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 aerospace_chatbot-0.0.4/PKG-INFO
```

### Comparing `aerospace_chatbot-0.0.3/LICENSE` & `aerospace_chatbot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aerospace_chatbot-0.0.3/pyproject.toml` & `aerospace_chatbot-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aerospace-chatbot"
-version = "0.0.3"
+version = "0.0.4"
 description = "Aerospace engineering chatbot and AI tools."
 authors = ["dsmueller <dsm@danmueller.pro>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dan-s-mueller/aerospace_chatbot/tree/main"
 repository = "https://github.com/dan-s-mueller/aerospace_chatbot/tree/main"
```

### Comparing `aerospace_chatbot-0.0.3/src/aerospace_chatbot/admin.py` & `aerospace_chatbot-0.0.4/src/aerospace_chatbot/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,42 +8,54 @@
 import streamlit as st
 from dotenv import load_dotenv,find_dotenv
 
 import openai
 from pinecone import Pinecone
 import chromadb
 from langchain_openai import ChatOpenAI
-import pytest
+
+from langchain_openai import OpenAIEmbeddings
+from langchain_voyageai import VoyageAIEmbeddings
+from langchain_community.embeddings import HuggingFaceInferenceAPIEmbeddings
 
 class SecretKeyException(Exception):
     """Exception raised for secret key related errors.
 
     Attributes:
         message -- explanation of the error
         id -- unique identifier for the error
     """
 
     def __init__(self, message, id):
         super().__init__(message)
         self.id = id
+class DatabaseException(Exception):
+    """Exception raised for database related errors.
+
+    Attributes:
+        message -- explanation of the error
+        id -- unique identifier for the error
+    """
+
+    def __init__(self, message, id):
+        super().__init__(message)
+        self.id = id
 def load_sidebar(config_file,
-                 index_data_file,
                  vector_database=False,
                  embeddings=False,
                  rag_type=False,
                  index_name=False,
                  llm=False,
                  model_options=False,
                  secret_keys=False):
     """
     Loads the sidebar configuration for the chatbot.
 
     Args:
         config_file (str): The path to the configuration file.
-        index_data_file (str): The path to the index data file.
         vector_database (bool, optional): Whether to include the vector database in the sidebar. Defaults to False.
         embeddings (bool, optional): Whether to include embeddings in the sidebar. Defaults to False.
         rag_type (bool, optional): Whether to include RAG type in the sidebar. Defaults to False.
         index_name (bool, optional): Whether to include index name in the sidebar. Defaults to False.
         llm (bool, optional): Whether to include LLM in the sidebar. Defaults to False.
         model_options (bool, optional): Whether to include model options in the sidebar. Defaults to False.
         secret_keys (bool, optional): Whether to include secret keys in the sidebar. Defaults to False.
@@ -51,97 +63,101 @@
     Returns:
         dict: The sidebar configuration.
     """
     sb_out={}
     with open(config_file, 'r') as f:
         config = json.load(f)
         databases = {db['name']: db for db in config['databases']}
+        embeddings_list = {e['name']: e for e in config['embeddings']}
         llms  = {m['name']: m for m in config['llms']}
-        logging.info('Loaded: '+config_file)
-    with open(index_data_file, 'r') as f:
-        index_data = json.load(f)
-        logging.info('Loaded: '+index_data_file)
 
     # Set local db path
     if os.getenv('LOCAL_DB_PATH') is None or os.getenv('LOCAL_DB_PATH')=='':
         # This is the case where the .env file is not in the directory
         raise SecretKeyException('Local Database Path is required. Use an absolute path for local, or /data for hugging face spaces.','LOCAL_DB_PATH_MISSING')
 
     # Vector databases
     if vector_database:
         st.sidebar.title('Vector database')
         sb_out['index_type']=st.sidebar.selectbox('Index type', list(databases.keys()), index=1,help='Select the type of index to use.')
         logging.info('Index type: '+sb_out['index_type'])
 
         if embeddings:
             # Embeddings
-            st.sidebar.title('Embeddings')
+            st.sidebar.title('Embeddings',help='See embedding leaderboard here for performance overview: https://huggingface.co/spaces/mteb/leaderboard')
             if sb_out['index_type']=='RAGatouille':    # Default to selecting hugging face model for RAGatouille, otherwise select alternates
                 sb_out['query_model']=st.sidebar.selectbox('Hugging face rag models', 
                                                         databases[sb_out['index_type']]['hf_rag_models'], 
                                                         index=0,
                                                         help="Models listed are compatible with the selected index type.")
+                sb_out['embedding_name']=sb_out['query_model']
             else:
-                sb_out['query_model']=st.sidebar.selectbox('Embedding models', 
+                sb_out['query_model']=st.sidebar.selectbox('Embedding model family', 
                                                         databases[sb_out['index_type']]['embedding_models'], 
                                                         index=0,
+                                                        help="Model provider.")
+                sb_out['embedding_name']=st.sidebar.selectbox('Embedding model', 
+                                                        embeddings_list[sb_out['query_model']]['embedding_models'], 
+                                                        index=0,
                                                         help="Models listed are compatible with the selected index type.")
-
-            if sb_out['query_model']=='Openai':
-                sb_out['embedding_name']='text-embedding-ada-002'
-            elif sb_out['query_model']=='Voyage':
-                sb_out['embedding_name']='voyage-02'
-            logging.info('Query type: '+sb_out['query_model'])
-            if 'embedding_name' in locals() or 'embedding_name' in globals():
-                logging.info('Embedding name: '+sb_out['embedding_name'])
+            
         if rag_type:
             # RAG Type
             st.sidebar.title('RAG Type')
             if sb_out['index_type']=='RAGatouille':
                 sb_out['rag_type']=st.sidebar.selectbox('RAG type', ['Standard'], index=0,help='Only Standard is available for RAGatouille.')
             else:
                 sb_out['rag_type']=st.sidebar.selectbox('RAG type', ['Standard','Parent-Child','Summary'], index=0,help='Parent-Child is for parent-child RAG. Summary is for summarization RAG.')
                 if sb_out['rag_type']=='Summary' or sb_out['rag_type']=='Muti-Query':
                     sb_out['rag_llm_source']=st.sidebar.selectbox('RAG LLM model', list(llms.keys()), index=0,help='Select the LLM model for RAG.')
                     if sb_out['rag_llm_source']=='OpenAI':
                         sb_out['rag_llm_model']=st.sidebar.selectbox('RAG OpenAI model', llms[sb_out['rag_llm_source']]['models'], index=0,help='Select the OpenAI model for RAG.')
                     if sb_out['rag_llm_source']=='Hugging Face':
-                        sb_out['hf_models']=llms['Hugging Face']['models']
                         sb_out['rag_llm_model']=st.sidebar.selectbox('RAG Hugging Face model', 
-                                                                [item['model'] for item in llms['Hugging Face']['models']], 
+                                                                llms['Hugging Face']['models'], 
                                                                 index=0,
                                                                 help='Select the Hugging Face model for RAG.')
                         sb_out['rag_hf_endpoint']='https://api-inference.huggingface.co/v1'
                     elif sb_out['rag_llm_source']=='LM Studio (local)':
                         sb_out['rag_llm_model']=st.sidebar.text_input('Local host URL',
                                                                 'http://localhost:1234/v1',
                                                                 help='See LM studio configuration for local host URL.')
                         st.sidebar.warning('You must load a model in LM studio first for this to work.')
             logging.info('RAG type: '+sb_out['rag_type'])
         if index_name:
             if embeddings and rag_type:
                 # Index Name 
                 st.sidebar.title('Index Name')  
-                sb_out['index_name']=index_data[sb_out['index_type']][sb_out['query_model']]
-                st.sidebar.markdown('Index base name: '+sb_out['index_name'],help='config/index_data.json contains index base names. An index appendix is added on creation under Database Processing.')
+                sb_out['index_name'] = (sb_out['index_type'] + '-' + sb_out['embedding_name'].replace('/', '-')).lower()
+                st.sidebar.markdown('Index base name: '+sb_out['index_name'],help='An index appendix is added on creation under Database Processing.')
                 logging.info('Index name: '+sb_out['index_name'])
                 
                 # For each index type, list indices available for the base name
                 if sb_out['index_type']=='ChromaDB':
                     indices=show_chroma_collections(format=False)
                     if indices['status']:
                         name=[]
                         for index in indices['message']:
-                            if sb_out['rag_type']=='Parent-Child':
-                                if index.name.endswith('parent-child'):
-                                    name.append(index.name)
-                            else:
-                                if not index.name.endswith('parent-child'):
+                            # Be compatible with embedding types already used. Pinecone only supports lowercase.
+                            if index.name.startswith((sb_out['index_type'] + '-' + sb_out['embedding_name'].replace('/', '-')).lower()):    
+                                if sb_out['rag_type']=='Parent-Child':
+                                    if index.name.endswith('-parent-child'):
+                                        name.append(index.name)
+                                elif sb_out['rag_type']=='Summary':
+                                    if index.name.endswith('-summary'):
+                                        name.append(index.name)
+                                else:
                                     name.append(index.name)
                         sb_out['index_selected']=st.sidebar.selectbox('Index selected',name,index=0,help='Select the index to use for the application.')
+                        try:
+                            if len(name) == 0:
+                                raise DatabaseException('No collections found for the selected index type/embedding. Create a new database, or select another index type/embedding.','NO_COMPATIBLE_COLLECTIONS')
+                        except DatabaseException as e:
+                            st.warning(f"{e}")
+                            st.stop()
                     else:
                         st.sidebar.markdown('No collections found.',help='Check the status on Home.')
                 elif sb_out['index_type']=='Pinecone':
                     indices=show_pinecone_indexes(format=False)
                     if indices['status']:
                         name=[]
                         for index in indices['message']:
@@ -157,23 +173,22 @@
                         sb_out['index_selected']=st.sidebar.selectbox('Index selected',name,index=0,help='Select the index to use for the application.')
                     else:
                         st.sidebar.markdown('No collections found.',help='Check the status on Home.')
             else:
                 raise ValueError('Embeddings must be enabled to select an index name.')
         if llm:
             # LLM
-            st.sidebar.title('LLM')
+            st.sidebar.title('LLM',help='See LLM leaderboard here for performance overview: https://huggingface.co/spaces/lmsys/chatbot-arena-leaderboard')
             sb_out['llm_source']=st.sidebar.selectbox('LLM model', list(llms.keys()), index=0,help='Select the LLM model for the application.')
             logging.info('LLM source: '+sb_out['llm_source'])
             if sb_out['llm_source']=='OpenAI':
                 sb_out['llm_model']=st.sidebar.selectbox('OpenAI model', llms[sb_out['llm_source']]['models'], index=0,help='Select the OpenAI model for the application.')
             elif sb_out['llm_source']=='Hugging Face':
-                sb_out['hf_models']=llms['Hugging Face']['models']
                 sb_out['llm_model']=st.sidebar.selectbox('Hugging Face model', 
-                                                        [item['model'] for item in llms['Hugging Face']['models']], 
+                                                        llms['Hugging Face']['models'], 
                                                         index=0,
                                                         help='Select the Hugging Face model for the application.')
                 sb_out['hf_endpoint']='https://api-inference.huggingface.co/v1'
             elif sb_out['llm_source']=='LM Studio (local)':
                 sb_out['llm_model']=st.sidebar.text_input('Local host URL',
                                                         'http://localhost:1234/v1',
                                                         help='See LM studio configuration for local host URL.')
@@ -347,14 +362,39 @@
         elif sb['rag_llm_source'] == 'LM Studio (local)':
             # base_url takes local configuration from lm studio, no api key required.
             llm = ChatOpenAI(base_url=sb['rag_llm_model'],
                              model_name='lm_studio')
         else:
             raise ValueError("Invalid LLM source specified.")
     return llm
+def get_query_model(sb, secrets):
+    """
+    Returns the query model based on the provided parameters.
+
+    Args:
+        sb (dict): A dictionary containing the parameters for the query model.
+        secrets (dict): A dictionary containing the API keys for different query models.
+
+    Returns:
+        query_model: The selected query model based on the provided parameters.
+
+    Raises:
+        NotImplementedError: If the query model is not recognized.
+    """
+    if sb['index_type'] == 'RAGatouille':
+        query_model = sb['query_model']
+    elif sb['query_model'] == 'OpenAI':
+        query_model = OpenAIEmbeddings(model=sb['embedding_name'], openai_api_key=secrets['OPENAI_API_KEY'])
+    elif sb['query_model'] == 'Voyage':
+        query_model = VoyageAIEmbeddings(model=sb['embedding_name'], voyage_api_key=secrets['VOYAGE_API_KEY'], truncation=False)
+    elif sb['query_model'] == 'Hugging Face':
+        query_model = HuggingFaceInferenceAPIEmbeddings(model_name=sb['embedding_name'], api_key=secrets['HUGGINGFACEHUB_API_TOKEN'])
+    else:
+        raise NotImplementedError('Query model not recognized.')
+    return query_model
 def show_pinecone_indexes(format=True):
     """
     Retrieves the list of Pinecone indexes and their status.
     LOCAL_DB_PATH environment variable used to pass the local database path.
 
     Args:
         format (bool, optional): Specifies whether to format the output. Defaults to True.
@@ -595,19 +635,17 @@
             warn_db_path.empty()
         except:
             pass    # If the text input has already been removed, do nothing
 
     # Load sidebar
     try:
         if sidebar_config is None:
-            sb=load_sidebar(config_file=os.path.join(config_folder_path,'config.json'),
-                            index_data_file=os.path.join(config_folder_path,'index_data.json'))
+            sb=load_sidebar(os.path.join(config_folder_path,'config.json'))
         else:
-            sb=load_sidebar(config_file=os.path.join(config_folder_path,'config.json'),
-                            index_data_file=os.path.join(config_folder_path,'index_data.json'),
+            sb=load_sidebar(os.path.join(config_folder_path,'config.json'),
                             **sidebar_config)
     except SecretKeyException as e:
         # If no .env file is found, set the local db path when the warning is raised.
         st.warning(f"{e}")
         st.stop()
     try:
         secrets=set_secrets(sb) # Take secrets from .env file first, otherwise from sidebar
```

### Comparing `aerospace_chatbot-0.0.3/src/aerospace_chatbot/data_processing.py` & `aerospace_chatbot-0.0.4/src/aerospace_chatbot/data_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,32 +24,34 @@
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
 from langchain.retrievers.multi_vector import MultiVectorRetriever
 from langchain.storage import LocalFileStore
 
 from langchain_openai import OpenAIEmbeddings
 from langchain_voyageai import VoyageAIEmbeddings
+from langchain_community.embeddings import HuggingFaceInferenceAPIEmbeddings
 
 from langchain_community.document_loaders import PyPDFLoader
 
 from langchain_core.documents import Document
 from langchain_core.output_parsers import StrOutputParser
 
 from ragatouille import RAGPretrainedModel
 
 from ragxplorer import RAGxplorer, rag
 import pandas as pd
 
 
 def load_docs(index_type:str,
-              docs,
-              query_model,
+              docs:List[str],
+              query_model:any,
+              embedding_name:str,
               rag_type:str='Standard',
               index_name:str=None,
-              n_merge_pages:int=0,
+              n_merge_pages:int=None,
               chunk_method:str='character_recursive',
               chunk_size:int=500,
               chunk_overlap:int=0,
               clear:bool=False,
               file_out:str=None,
               batch_size:int=50,
               local_db_path:str='.',
@@ -58,14 +60,15 @@
     """
     Loads documents into the specified index.
 
     Args:
         index_type (str): The type of index to use.
         docs: The documents to load.
         query_model: The query model to use.
+        embedding_name: The name of the embedding model to use.
         rag_type (str, optional): The type of RAG (Retrieval-Augmented Generation) to use. Defaults to 'Standard'.
         index_name (str, optional): The name of the index. Defaults to None.
         n_merge_pages (int, optional): Number of pages to to merge when loading. Defaults to 0.
         chunk_method (str, optional): The method to chunk the documents. Defaults to 'character_recursive'.
         chunk_size (int, optional): The size of each chunk. Defaults to 500.
         chunk_overlap (int, optional): The overlap between chunks. Defaults to 0.
         clear (bool, optional): Whether to clear the index before loading new documents. Defaults to False.
@@ -93,20 +96,21 @@
                        llm=llm,
                        show_progress=show_progress)
         
     # Set index names for special databases
     if rag_type == 'Parent-Child':
         index_name = index_name + '-parent-child'
     if rag_type == 'Summary':
-        index_name = index_name + '-summary-' + llm.model_name.replace('/', '-')
+        index_name = index_name + llm.model_name.replace('/', '-') + '-summary' 
 
     # Initialize client an upsert docs
     vectorstore = initialize_database(index_type, 
                                       index_name, 
                                       query_model, 
+                                      embedding_name,
                                       rag_type=rag_type,
                                       clear=clear, 
                                       local_db_path=local_db_path,
                                       init_ragatouille=True,
                                       show_progress=show_progress)
     vectorstore, retriever = upsert_docs(index_type,
                                          index_name,
@@ -190,15 +194,15 @@
             page_chunks = text_splitter.split_documents(pages)
             for i, chunk in enumerate(page_chunks):
                 if show_progress:
                     progress_percentage = i / len(page_chunks)
                     my_bar.progress(progress_percentage, text=f'Chunking documents...{progress_percentage*100:.2f}%')
                 chunk.page_content += str(chunk.metadata)    # Add metadata to the end of the page content, some RAG models don't have metadata.
                 chunks.append(chunk)    # Not sanitized because the page already was
-        elif chunk_method is 'None':
+        elif chunk_method=='None':
             text_splitter = None
             chunks = pages  # No chunking, take whole pages as documents
         else:
             raise NotImplementedError
         
         if file_out:
             # Write to a jsonl file, save it.
@@ -218,15 +222,15 @@
         if chunk_method=='character_recursive':
             parent_splitter=RecursiveCharacterTextSplitter(chunk_size=chunk_size*k_parent, 
                                                            chunk_overlap=chunk_overlap,
                                                            add_start_index=True)    # Without add_start_index, will not be a unique id
             child_splitter=RecursiveCharacterTextSplitter(chunk_size=chunk_size, 
                                                           chunk_overlap=chunk_overlap,
                                                           add_start_index=True)
-        elif chunk_method is 'None':
+        elif chunk_method=='None':
             raise ValueError("You must specify a chunk_method with rag_type=Parent-Child.")
         else:
             raise NotImplementedError
         
         # Split up parent chunks
         parent_chunks = parent_splitter.split_documents(pages)
         doc_ids = [str(_stable_hash_meta(parent_chunk.metadata)) for parent_chunk in parent_chunks]
@@ -279,26 +283,28 @@
                 'pages':{'doc_ids':doc_ids,'docs':pages},
                 'summaries':summary_docs,
                 'llm':llm}
     else:
         raise NotImplementedError
 def initialize_database(index_type: str, 
                         index_name: str, 
-                        query_model: str, 
+                        query_model: str,
+                        embedding_name: str,
                         rag_type: str,
                         local_db_path: str = None, 
                         clear: bool = False,
                         init_ragatouille: bool = False,
                         show_progress: bool = False):
     """Initializes the database based on the specified parameters.
 
     Args:
         index_type (str): The type of index to use (e.g., "Pinecone", "ChromaDB", "RAGatouille").
         index_name (str): The name of the index.
         query_model (str): The query model to use.
+        embedding_name (str): The name of the embedding model to use.
         rag_type (str): The type of RAG model to use.
         local_db_path (str, optional): The path to the local database. Defaults to None.
         clear (bool, optional): Whether to clear the index. Defaults to False.
         init_ragatouille (bool, optional): Whether to initialize the RAGatouille model. Defaults to False.
         show_progress (bool, optional): Whether to show the progress bar. Defaults to False.
 
     Returns:
@@ -318,15 +324,15 @@
             delete_index(index_type, index_name, rag_type, local_db_path=local_db_path)
         pc = pinecone_client(api_key=os.getenv('PINECONE_API_KEY'))
         
         try:
             pc.describe_index(index_name)
         except:
             pc.create_index(index_name,
-                            dimension=_embedding_size(query_model),
+                            dimension=_embedding_size(query_model,embedding_name),
                             spec=PodSpec(environment="us-west1-gcp", pod_type="p1.x1"))
         
         index = pc.Index(index_name)
         vectorstore=PineconeVectorStore(index,
                                         index_name=index_name, 
                                         embedding=query_model,
                                         text_key='page_content',
@@ -362,87 +368,66 @@
     return vectorstore
 
 @retry(stop=stop_after_attempt(15), wait=wait_exponential(multiplier=1,max=60))
 def upsert_docs_pinecone(index_name: str,
                          vectorstore: any, 
                          chunker: dict, 
                          batch_size: int = 50, 
-                         show_progress: bool = False,
                          local_db_path: str = '.'):
     """
     Upserts documents into Pinecone index. Refactored spearately from upsert_docs to allow for tenacity retries.
 
     Args:
         index_name (str): The name of the Pinecone index.
         vectorstore (any): The vectorstore object for storing the document vectors.
         chunker (dict): The chunker object containing the documents to upsert.
         batch_size (int, optional): The number of documents to upsert in each batch. Defaults to 50.
-        show_progress (bool, optional): Whether to show progress bar during upsert. Defaults to False.
         local_db_path (str, optional): The path to the local database. Defaults to '.'.
 
     Returns:
         tuple: A tuple containing the updated vectorstore and retriever objects.
     """
     
-    if show_progress:
-        progress_text = "Upsert in progress..."
-        my_bar = st.progress(0, text=progress_text)
-    
     if chunker['rag'] == 'Standard':
         for i in range(0, len(chunker['chunks']), batch_size):
             chunk_batch = chunker['chunks'][i:i + batch_size]
             chunk_batch_ids = [_stable_hash_meta(chunk.metadata) for chunk in chunk_batch]   # add ID which is the hash of metadata
             vectorstore.add_documents(documents=chunk_batch,
                                         ids=chunk_batch_ids)
-            if show_progress:
-                progress_percentage = i / len(chunker['chunks'])
-                my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')
         retriever = vectorstore.as_retriever()
     elif chunker['rag'] == 'Parent-Child':
         lfs_path = Path(local_db_path).resolve() / 'local_file_store' / index_name
         store = LocalFileStore(lfs_path)
         
         id_key = "doc_id"
         retriever = MultiVectorRetriever(vectorstore=vectorstore, byte_store=store, id_key=id_key)
 
         for i in range(0, len(chunker['chunks']), batch_size):
             chunk_batch = chunker['chunks'][i:i + batch_size]
             chunk_batch_ids = [_stable_hash_meta(chunk.metadata) for chunk in chunk_batch]   # add ID which is the hash of metadata
             retriever.vectorstore.add_documents(documents=chunk_batch,
                                                 ids=chunk_batch_ids)
-            if show_progress:
-                progress_percentage = i / len(chunker['chunks'])
-                my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')
-        
         # Index parent docs all at once
         retriever.docstore.mset(list(zip(chunker['pages']['doc_ids'], chunker['pages']['parent_chunks'])))
     elif chunker['rag'] == 'Summary':
         lfs_path = Path(local_db_path).resolve() / 'local_file_store' / index_name
         store = LocalFileStore(lfs_path)
         
         id_key = "doc_id"
         retriever = MultiVectorRetriever(vectorstore=vectorstore, byte_store=store, id_key=id_key)
 
         for i in range(0, len(chunker['summaries']), batch_size):
             chunk_batch = chunker['summaries'][i:i + batch_size]
             chunk_batch_ids = [_stable_hash_meta(chunk.metadata) for chunk in chunk_batch]   # add ID which is the hash of metadata
             retriever.vectorstore.add_documents(documents=chunk_batch,
                                                 ids=chunk_batch_ids)
-            if show_progress:
-                progress_percentage = i / len(chunker['summaries'])
-                my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')
-        
         # Index parent docs all at once
         retriever.docstore.mset(list(zip(chunker['pages']['doc_ids'], chunker['pages']['docs'])))
     else:
         raise NotImplementedError
-    
-    if show_progress:
-        my_bar.empty()
-
     return vectorstore, retriever
         
 def upsert_docs(index_type: str, 
                 index_name: str,
                 vectorstore: any, 
                 chunker: dict, 
                 batch_size: int = 50, 
@@ -466,19 +451,21 @@
     if show_progress:
         progress_text = "Upsert in progress..."
         my_bar = st.progress(0, text=progress_text)
 
     if chunker['rag'] == 'Standard':
         # Upsert each chunk in batches
         if index_type == "Pinecone":
+            if show_progress:
+                progress_text = "Upsert in progress to Pinecone..."
+                my_bar.progress(0, text=progress_text)
             vectorstore, retriever=upsert_docs_pinecone(index_name,
                                                         vectorstore, 
                                                         chunker, 
                                                         batch_size, 
-                                                        show_progress,
                                                         local_db_path)
         elif index_type == "ChromaDB":
             for i in range(0, len(chunker['chunks']), batch_size):
                 chunk_batch = chunker['chunks'][i:i + batch_size]
                 chunk_batch_ids = [_stable_hash_meta(chunk.metadata) for chunk in chunk_batch]   # add ID which is the hash of metadata
                 vectorstore.add_documents(documents=chunk_batch,
                                           ids=chunk_batch_ids)
@@ -503,14 +490,17 @@
             except shutil.Error:
                 pass    # If it already exists, don't do anything
             retriever = vectorstore.as_langchain_retriever()
         else:
             raise NotImplementedError
     elif chunker['rag'] == 'Parent-Child':
         if index_type == 'Pincone':
+            if show_progress:
+                progress_text = "Upsert in progress to Pinecone..."
+                my_bar.progress(0, text=progress_text)
             vectorstore, retriever=upsert_docs_pinecone(index_name,
                                                         vectorstore, 
                                                         chunker, 
                                                         batch_size, 
                                                         show_progress,
                                                         local_db_path)
         elif index_type == 'ChromaDB':
@@ -533,14 +523,17 @@
             retriever.docstore.mset(list(zip(chunker['pages']['doc_ids'], chunker['pages']['parent_chunks'])))
         elif index_type == "RAGatouille":
             raise Exception('RAGAtouille only supports standard RAG.')
         else:
             raise NotImplementedError
     elif chunker['rag'] == 'Summary':
         if index_type == 'Pincone':
+            if show_progress:
+                progress_text = "Upsert in progress to Pinecone..."
+                my_bar.progress(0, text=progress_text)
             vectorstore, retriever=upsert_docs_pinecone(index_name,
                                                         vectorstore, 
                                                         chunker, 
                                                         batch_size, 
                                                         show_progress,
                                                         local_db_path)
         elif index_type == 'ChromaDB':
@@ -809,33 +802,58 @@
     if len(text) == 0:
         return None
     alphanumeric_pct = sum(c.isalnum() for c in text) / len(text)
     if num_words < 5 or alphanumeric_pct < 0.3:
         return None
     else:
         return page
-def _embedding_size(embedding_model:any):
+def _embedding_size(embedding_family:any,embedding_name:str):
     """
     Returns the size of the embedding for a given embedding model.
 
     Args:
-        embedding_model (object): The embedding model to get the size for.
+        embedding_family (object): The embedding model to get the size for.
+        embedding_name (str): The name of the embedding model.
 
     Returns:
         int: The size of the embedding.
 
     Raises:
         NotImplementedError: If the embedding model is not supported.
     """
-    if isinstance(embedding_model,OpenAIEmbeddings):
-        return 1536 # https://platform.openai.com/docs/models/embeddings, test-embedding-ada-002
-    elif isinstance(embedding_model,VoyageAIEmbeddings):
-        return 1024 # https://docs.voyageai.com/embeddings/, voyage-02
+    exception_embedding_name=NotImplementedError(f"The embedding name '{embedding_name}' is not available in config.json")
+
+    # https://platform.openai.com/docs/models/embeddings
+    if isinstance(embedding_family,OpenAIEmbeddings):
+        if embedding_name=="text-embedding-ada-002":
+            return 1536
+        elif embedding_name=="text-embedding-3-small":
+            return 1536
+        elif embedding_name=="text-embedding-3-large":
+            return 3072
+        else:
+            raise exception_embedding_name
+    # https://docs.voyageai.com/embeddings/
+    elif isinstance(embedding_family,VoyageAIEmbeddings):
+        if embedding_name=="voyage-2":
+            return 1024 
+        elif embedding_name=="voyage-large-2":
+            return 1536
+        else:
+            raise exception_embedding_name
+    # See model pages for embedding sizes
+    elif isinstance(embedding_family,HuggingFaceInferenceAPIEmbeddings):
+        if embedding_name=="sentence-transformers/all-MiniLM-L6-v2":
+            return 384
+        elif embedding_name=="mixedbread-ai/mxbai-embed-large-v1":
+            return 1024
+        else:
+            raise exception_embedding_name
     else:
-        raise NotImplementedError
+        raise NotImplementedError(f"The embedding family '{embedding_family}' is not available in config.json")
 
 def _stable_hash_meta(metadata: dict) -> str:
     """
     Stable hash of metadata from Langchain Document.
 
     Args:
         metadata (dict): The metadata dictionary to be hashed.
```

### Comparing `aerospace_chatbot-0.0.3/src/aerospace_chatbot/prompts.py` & `aerospace_chatbot-0.0.4/src/aerospace_chatbot/prompts.py`

 * *Files identical despite different names*

### Comparing `aerospace_chatbot-0.0.3/src/aerospace_chatbot/queries.py` & `aerospace_chatbot-0.0.4/src/aerospace_chatbot/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,40 +70,43 @@
         conversational_qa_chain (Chain): The chain for conversational QA.
 
     """
     def __init__(self, 
                  index_type,
                  index_name,
                  query_model,
+                 embedding_name,
                  llm:ChatOpenAI,
                  rag_type='Standard',
                  k=6,
                  search_type='similarity',
                  fetch_k=50,
                  temperature=0,
                  local_db_path='.'):
         """
         Initializes a new instance of the QA_Model class.
 
         Args:
             index_type (str): The type of index.
             index_name (str): The name of the index.
             query_model (str): The query model.
+            embedding_name (str): The name of the embedding.
             llm (ChatOpenAI): The language model for generating responses.
             rag_type (str, optional): The type of RAG model. Defaults to 'Standard'.
             k (int, optional): The number of retriever results to consider. Defaults to 6.
             search_type (str, optional): The type of search to perform. Defaults to 'similarity'.
             fetch_k (int, optional): The number of documents to fetch from the retriever. Defaults to 50.
             temperature (int, optional): The temperature for response generation. Defaults to 0.
             local_db_path (str, optional): The path to the local database. Defaults to '.'.
 
         """
         self.index_type=index_type
         self.index_name=index_name
         self.query_model=query_model
+        self.embedding_name=embedding_name
         self.llm=llm
         self.rag_type=rag_type
         self.k=k
         self.search_type=search_type
         self.fetch_k=fetch_k
         self.temperature=temperature
         self.local_db_path=local_db_path
@@ -114,14 +117,15 @@
                                                 self.k,
                                                 self.fetch_k)
 
         # Read in from the vector database
         self.vectorstore=data_processing.initialize_database(self.index_type,
                                                              self.index_name,
                                                              self.query_model,
+                                                             self.embedding_name,
                                                              self.rag_type,
                                                              local_db_path=self.local_db_path,
                                                              init_ragatouille=False)  
         if self.rag_type=='Standard':  
             if self.index_type=='ChromaDB' or self.index_type=='Pinecone':
                 self.retriever=self.vectorstore.as_retriever(search_type=self.search_type)
             elif self.index_type=='RAGatouille':
```

### Comparing `aerospace_chatbot-0.0.3/PKG-INFO` & `aerospace_chatbot-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospace-chatbot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Aerospace engineering chatbot and AI tools.
 Home-page: https://github.com/dan-s-mueller/aerospace_chatbot/tree/main
 License: MIT
 Author: dsmueller
 Author-email: dsm@danmueller.pro
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*, !=3.12.*
 Classifier: License :: OSI Approved :: MIT License
```

