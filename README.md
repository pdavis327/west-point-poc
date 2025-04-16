# west-point-poc

## Prerequisites
To set up a new Conda environment, run the following commands:

```zsh
conda create --name westpoint python==3.11
conda activate westpoint
pip install -r requirements.txt
```

To add pre-commit hooks, run the following command:
```zsh
`pre-commit install`
```

## Repository structure
The following are files and folders in the repository:

* `requirements.txt`: This file contains python dependencies.
* `util/`: This folder contains some utility modules.
* `assets/raw_data`: This folder contains the original pdfs.
* `assets/docling_out`: This directory contains the docling converted .md documents.
* `taxonomy/qna`: Contains the QnA files for InstructLab fine tuning.

## Convert .pdf to .md using docling
```console
cd util
python convert_pdf.py ./assets/raw_data ./assets/docling_out
```
