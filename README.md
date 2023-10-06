This template is customized from a book tittled **Good Research Code handbook**.

## Clone this repository
git clone https://github.com/alannguyencs/code_template.git

## Rename the two folders code_template

## Create a new conda environment
```
conda create -n code_template_env python=3.8
conda activate code_template_env
```

## Enter the folders and open by visual studio
```
cd code_template
code .
```

## Export conda environment
```
conda env export > environment.yml
```


## pip install your package
```
pip install -e .
```