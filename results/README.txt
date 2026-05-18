Here is the directory containing the files related to the LLM-based screening experiment.

The files are organized as follows:

root--------------------------#project root
├ code------------------------#Python scripts used for execution
|  ├ analysis.py--------------#main script for LLM application
|  ├ compare.py---------------#comparison results builder
|  └ prompt.py----------------#prompt builder
├ prompts---------------------#prompt history
└ study-----------------------#results for each study
  ├ model---------------------#model used
  |  └ comparison_vN.txt------#comparison against ground truth (N denotes the prompt version)
  └ start_data----------------#ground truth data
      ├ articles.json---------#analyzed titles and abstracts
      ├ criteria.json---------#inclusion and exclusion criteria
      └ ground_truth.json-----#original results