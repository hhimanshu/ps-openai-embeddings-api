# Installation
- You must install [Conda](https://docs.conda.io/projects/conda/en/stable/). Please select the install methods that suits your Operating System.
- Open Terminal and run the following commands:
### Create a conda environment
```sh
conda create -n ps python=3.11
```

### Activate the environment
```sh
conda activate ps
```
### Install ipykernel
```sh

conda install anaconda::ipykernel
```

With these changes, you now have an environment that is ready to run the Jupyter Notebook.

### Setup Open AI API key
- Sign up on [Open AI Platform](https://platform.openai.com/) and create an API key.
- Create `.env` file
```sh
cp .env.sample .env
```
- Replace "my_key" with the API key obtained from Open AI Platform


## Other commands
### List all environments
```sh
conda env list
```

### Remove an environment
```sh
conda remove --name ps --all
```

## How input file is created?
- Download the input file from [here](https://www.kaggle.com/datasets/muhammadahmedansari/airbnb-dataset?resource=download)
- Unzip the file
```sh
unzip archive.zip
```

- Run the following commands
```sh
head -200 data/input/reviews.csv > data/input/reviews_200.csv
```