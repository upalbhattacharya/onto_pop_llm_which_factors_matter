# Run Arguments

The various parameters used for experimenting with different
LLMs, domain contexts, n-shot prompting approaches and
temperature settings can be found in `json` files here. The 
provided directory structure below explains how the data is categorized.
Each `uuid-x.json` corresponds to a domain context variant. The same 
UUID can be found in the [results](../results) directory for the
corresponding results.

```
.
├── embeddings : Parameters for generating OpenAI embeddings
│   ├── Ontology Name
│   │   ├── concepts_no_processing.json : Parameters for generating embeddings for concepts of ontology
│   │   └── individuals_no_processing.json : Parameters for generating embeddings for individuals of ontology
├── onto_pop : Parameters for Ontology Population Experiments
│   ├── 0_shot
│   │   ├── LLM Name
│   │   │   ├── Ontology Name
│   │   │   │   ├── uuid-1.json : Parameters for one domain context
│   │   │   │   ├── uuid-2.json
│   │   │   │   ├── uuid-3.json
│   │   │   │   └── uuid-4.json
│   │   │   │      
│   │   ├── 3_shot
│   │   │   ├── LLM Name
│   │   │   │   ├── Ontology Name
│   │   │   │   │   ├── uuid-5.json
│   │   │   │   │   ├── uuid-6.json
│   │   │   │   │   ├── uuid-7.json
│   │   │   │   │   ├── uuid-8.json
│   │   │   │   │   ├── t0.0.json
│   │   │   │   │   ├── t0.2.json
│   │   │   │   │   ├── t0.4.json
│   │   │   │   │   ├── t0.6.json
│   │   │   │   │   ├── t0.8.json
│   │   │   │   │   └── t1.0.json
```
