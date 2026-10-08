# CO 3 — Complete textbook notebook

Open **[CO3_Complete_Textbook_Notes.ipynb](CO3_Complete_Textbook_Notes.ipynb)** in VS Code or Jupyter. For a browser-readable companion, open **[CO3_Complete_Textbook_Notes.html](CO3_Complete_Textbook_Notes.html)**. Notebook figures and executed outputs are embedded; the HTML embeds images, while mathematical typesetting may use the renderer's external MathJax resource.

The book covers all eight requested topics: VANETs, IoV, edge computing, fog computing, cloud-based architectures, middleware frameworks, data synchronization, and consistency in distributed autonomous systems.

It includes 24 fully worked numerical problems, 11 original architecture diagrams, eight plotted executable laboratories, eight topic case studies, an integrated shuttle design, a documented Spanner research case, 16 developed examination answers, eight additional practice numericals, a formula sheet, glossary and 19 source entries. Hypothetical examples are explicitly distinguished from documented research.

## Files

- `CO3_Complete_Textbook_Notes.ipynb`: main executed notebook.
- `CO3_Complete_Textbook_Notes.html`: reading companion.
- `content/`: editable chapter sources; these are not the final notebook.
- `figures/`: original architecture figures, also embedded in the notebook.
- `tools/build_notebook.py`: regenerates figures, notebook, execution outputs, HTML and summary.
- `tools/validate_notebook.py`: checks the saved artifact independently.
- `validation_report.json`: counts and execution status from the build.

## Run or rebuild

From this folder with Python 3:

```powershell
python -m pip install -r requirements.txt
python tools/build_notebook.py
python tools/validate_notebook.py
```

For interactive execution, use the Python 3 kernel and select **Run All**. Ten code cells comprise setup, eight topic labs and arithmetic verification. The labs need NumPy, Matplotlib and IPython, and use no network services or credentials. Build tools additionally require the notebook packages listed in `requirements.txt`.

Successful execution verifies the toy calculations, not a deployed autonomous system or a full protocol implementation. Source access limitations and edition boundaries are documented in the notebook bibliography.
