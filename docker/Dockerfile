FROM continuumio/miniconda3
RUN conda install jupyterlab
# need latest jupyterlab to use altair
RUN conda update jupyterlab
RUN conda install geopandas
RUN pip install gpdvega
RUN pip install us
RUN pip install census
RUN conda install seaborn
RUN conda install scikit-learn
RUN conda install -c conda-forge altair vega_datasets
RUN conda install -c conda-forge descartes
RUN conda install -c conda-forge/label/cf202003 nodejs
RUN pip install jupyterlab_vim
RUN conda install openpyxl
CMD jupyter lab --notebook-dir=/opt/laurelhurst4all --ip='0.0.0.0' --port=8877 --no-browser --allow-root
