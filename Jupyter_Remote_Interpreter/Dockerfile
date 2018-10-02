FROM jupyter/minimal-notebook
WORKDIR /opt
COPY requirements.txt /opt/requirements.txt
RUN pip install -r /opt/requirements.txt
COPY src /home/jovyan/work
EXPOSE 8888
ENTRYPOINT jupyter-notebook --no-browser --ip='0.0.0.0' --port=8888 --allow-root --NotebookApp.token='' --NotebookApp.notebook_dir="/home/jovyan"