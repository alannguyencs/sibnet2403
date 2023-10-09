This template is customized from a book tittled **Good Research Code handbook**.

## Clone this repository
```
git clone https://github.com/alannguyencs/code_template.git
```

## Remove remote url
```
git remote rm origin
```

## Rename the two folders code_template

## Create a new conda environment
```
conda create -n code_template_env python=3.8
conda activate code_template_env
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
```

## Enter the folders and open by visual studio
```
cd code_template
code .
```
In Visual studio, press Ctrl + Shift + P to change the Conda environment interpreter

## Export conda environment
```
conda env export > environment.yml
```


## pip install your package
```
pip install -e .
```

## Add the environment as a kernel to Jupyter Notebook:
```
python -m ipykernel install --user --name=your-env
```

## Frequent used commands
+ Check git size: `git count-objects -vH`
+ Export conda environment: `conda env export > environment.yml`
+ Update conda environment from submodules: 
	+ Go to submodule and install it: `pip install -e .`
	+ `conda env update --name code_template_env -f environment.yml --prune`