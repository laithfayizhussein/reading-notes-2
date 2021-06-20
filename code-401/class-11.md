# Data Science

- It is a set of disciplines and practices that handle data in a scientific manner. The foundations of data science are mostly Mathematics and Statistics, sometimes Software Engineering would play a role as well
there are some definitions for the data science :

>“Data science is an interdisciplinary field about processes and systems to extract knowledge or insights from data in various forms, either structured or unstructured, which is a continuation of some of the data analysis fields such as statistics, data mining, and predictive analytics, similar to Knowledge Discovery in Databases.” – Wikipedia

> “The science of dealing with data, once they have been established, while the relation of the data to what they represent is delegated to other fields and sciences.” – Peter Naur

>“By ‘Data Science’ we mean almost everything that has something to do with data: Collecting, analyzing, modeling…” – The Journal of Data Science
- Usually, it includes but not limited to these steps:
    - Data acquisition : To play with data, you need to have data first.
        The data could be in the form of .CSV files. Excel file (.XLSX) is a typical form, or it could be available by API calls, or someone has done the dirty work already and they are all in DWH(Data WareHouse) or Data Lake.
    - Data cleaning & wrangling : In the actual working environment, data is rarely ready to be used right away.
        Data could be in the nested structure for storage saving purpose (e.g. Bigquery and NoSQL), could be normalized (like general databases). The data need to be flattened before usage.
   - Data Engineering : It is a extremely vital part as all kinds of data science tricks depends on it.
        If there is no good data to use, NONE of the data science gimmicks could work.
        Well engineered data should be clean, fast and cheap (in terms of computational resources, hence money as well) for robust consumption right away.
    - Utilization of data : This is the sexy part that people couldn’t stop talking about.
        From traditional consumption like building an application, doing ad hoc analysis, dashboarding and the recent fancy thing such as Machine Learning, this is the step people care so much.


# What is Jupyter Lab

- JupyterLab is a next-generation web-based user interface for Project Jupyter.

- JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner.

- You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing.

- Code Consoles provide transient scratchpads for running code interactively, with full support for rich output. A code console can be linked to a notebook kernel as a computation log from the notebook, for example.

- Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.

- Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

- Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. For example, it is easy to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.

- JupyterLab also offers a unified model for viewing and handling data formats. JupyterLab understands many file formats (images, CSV, JSON, Markdown, PDF, Vega, Vega-Lite, etc.) and can also display rich kernel output in these formats. See File and Output Formats for more information.

- To navigate the user interface, JupyterLab offers customizable keyboard shortcuts and the ability to use key maps from vim, emacs, and Sublime Text in the text editor.

- JupyterLab extensions can customize or enhance any part of JupyterLab, including new themes, file editors, and custom components.

- JupyterLab is served from the same server and uses the same notebook document format as the classic Jupyter Notebook.
