python3 -m venv env

source env/bin/activate

pip install pandas numpy statsmodels
pip install scikit-learn
pip install matplotlib seaborn
pip install ipython jupyterlab notebook
pip install imbalanced-learn
pip install graphviz


#Jupyter Kernal
Register virtual env as Kernal
    python -m ipykernel install --user --name=env --display-name "Python (env)"
