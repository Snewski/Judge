# Judge

This project evaluates large language models as automated judges for complex, rule‑based decision‑making in a trading‑card game environment. It compares a baseline model against a retrieval‑augmented model to assess how additional contextual information—such as card text and rulebook excerpts—affects the accuracy and consistency of model‑generated rulings and explanations.

To run the Notebooks in src folder, due the following:

1. Run the setup.sh to create a virtual environment
2. Activate the environment with: source .venv/bin/activate
3. Attach the environment with: python3 -m ipykernel install --user --name=.venv

The src folder contains 4 notebooks & 1 R-markdown file that does the following:
1. Test_data.ipynb: Is used to create a test dataset, new entries can easily be added by following the given structure.
2. Baseline_Judge.ipynb: Is used to generate rulings & explanations for the test dataset, using only the game state and a query.
3. RAG_Judge.ipynb: Is used to generate rulings & explanations for the test dataset, using the game state, card text, retrieved context, and a query.
4. Visualizations.ipynb: Simply makes some visualization of the results.
5. Table.Rmd: Is used to create a latex table comparing rulings and explanations. 
