# Ontology Population Using LLMs: Which Factors Matter?

This is the repository containing all relevant code, data, results and
additional tables and figures for the ESWC 2026 Research Track Paper:
**Ontology Population Using LLMs: Which Factors Matter?**

An outline of the repository is given below:
- The paper PDF can be found [here](paper.pdf).
- Additional Tables and Figures for results of all experimentation 
  can be found [here](tables_and_figures.pdf).
- An Appendix containing the formulation of our Evaluation Metrics and an
  illustration of the preference for string similarity by LLMs when predicting
  hierarchies can be found [here](appendix.pdf).
- The data including the ontology files along with the zero-shot
  and few-shot datasets can be found in the [data](data/) directory.
- All relevant source code for pre-processing data, running experiments
  on various LLMs and calculating metrics can be found in the 
  [src/eswc\_2026\_submission\_13](src/onto_pop_llm_which_factors_matter/)
  directory and the [notebooks](notebooks/) directory.
  - An overview of the prompts used in experimentation can be found in the
    [prompt_templates](prompt_templates/) directory.
- The various settings for experiments with different factors can be found
  in the [run\_args](run_args/) directory.
- The generated results can be found in the [results](results/)
  directory.
