# Prompt Templates

The generic template for 0 shot and n shot prompts can be found in
[0_shot.md](0_shot.md) and [n_shot.md](n_shot.md) respectively. Fields in
braces `{}` represent values to be filled. Several values that can be used to
populate a field are separate by forward slashes `/` (e.g. 4 types of domain
contextualization).

`ontology-description` in the templates represent the description provided for
the domain contextualization variant for each ontology. The table below
provides the exact text used for the domain context `ontology-description` for
each ontology:

| Ontology  | `ontology-description`     |
|-----------|----------------------------|
| Wines     | "wine expert"              |
| CASE      | "cyber crime investigator" |
| Astronomy | "astronomy expert"         |

`ontology-depth` in the templates are populated with the respective depth of
the ontology.

`classes` in the templates are populated with a flat-list of comma-separated
labels of the concepts of the ontology.

`examples` in the [n_shot](n_shot.md) prompt are populated with the selected
examples for n-shot prompts.

The **EXACT** prompts used for each combination of prompting approach, LLM,
ontology and domain contextualization can be found in the `system_message`
field of the `JSON` files in the [run_args/onto_pop](../run_args/onto_pop/)
directory which are grouped by prompting approach (0_shot, 1_shot, ...),
followed by LLM name and finally ontology. Four variants corresponding to
different domain contextualizations are can be found within the ontology
sub-directories.


```
.
├── 0_shot
│   ├── deepseekr1-distill-llama3-8B
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   ├── llama3-8B
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── o1-preview
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       ├── wines-ontology
│       └── wines-ontology_bckp
├── 10_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 1_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 2_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 3_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 4_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 5_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 6_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 7_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
├── 8_shot
│   ├── gpt-4o
│   │   ├── astronomy-ontology
│   │   ├── case-uco-owl-trafficking
│   │   └── wines-ontology
│   └── llama3-8B
│       ├── astronomy-ontology
│       ├── case-uco-owl-trafficking
│       └── wines-ontology
└── 9_shot
    ├── gpt-4o
    │   ├── astronomy-ontology
    │   ├── case-uco-owl-trafficking
    │   └── wines-ontology
    └── llama3-8B
        ├── astronomy-ontology
        ├── case-uco-owl-trafficking
        └── wines-ontology
``` 
