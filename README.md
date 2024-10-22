# dhlab-app-concordance

This repository contains source code for [the Concordance app](https://dh.nb.no/run/konkordans/) from DH-lab at the National Library of Norway (NLN).

The app allow users to retrieve short snippets of texts with keywords in context (KWIC), based on a tailored corpus of texts from NLN's collection.

Users can define the corpus by uploading an Excel file with metadata for the texts, or by defining a corpus in the sidebar. After the corpus definition is set, users can search for keywords in the corpus and get a list of KWIC. The KWICs can be downloaded as an Excel file.

## dhlab package and Streamlit

The app is built around the [`dhlab` package for python](https://pypi.org/project/dhlab/). `dhlab` provides various functionality to analyse text from NLN's digital collection, and a wrapper to retrieve text data through our [Swagger API](https://api.nb.no/dhlab/).

The webapp is published using [Streamlit](https://www.streamlit.io).