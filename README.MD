# PENELOPIE: Parallel EN-EL Open Information Extraction

This is a simple Jupyter notebook with a demo implementation of the "PENELOPIE: Enabling Open Information Extraction for the Greek Language through Machine Translation" paper, to be presented in EACL 2021 SRW.

## Prerequisites

* Python 3.6.9
* The Python wrapper of [OpenIE5](https://github.com/vaibhavad/python-wrapper-OpenIE5)  (has to be installed manually)
* The Python wrapper of [ClausIE](https://github.com/AnthonyMRios/pyclausie) (has to be installed from source)
* Follow the instructions below for additional requirements.


## Installation
1. It is recommended to create a new virtual environment to avoid version conflicts. For Linux:
```bash
python3 -m venv penelopie
source penelopie/bin/activate
```
2. Install the OpenIE5 and ClausIE OIE engines following the above links.
3. Install additional requirements with:
```bash
git clone https://github.com/lighteternal/PENELOPIE.git
cd PENELOPIE
pip install -r requirements.txt
```
## Usage
The pipeline showcased in the Jupyter notebook will process the Greek sentences in `data/demo_greek.txt`, translate them into English, extract triples using 3 OIE engines and back-translate the resulting triples in Greek. The results are found in `data/final_triples.csv`.
The standalone NMT models (EN2EL, EL2EN) can be found here: https://huggingface.co/lighteternal

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## License
[Apache2.0](https://choosealicense.com/licenses/apache-2.0/)
