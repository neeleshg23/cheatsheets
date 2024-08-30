# Jupyter Cheatsheet

Expose a Jupyter server within a private network:
- `conda install -y jupyter`
- `jupyter notebook --generate-config`
- `vim ~/.jupyter/jupyter_notebook_config.py`
- - Uncomment `c.NotebookApp.allowed_origin` and set it to `*`
  - Uncomment `c.NotebookApp.ip` and set it to `{SERVER ADDRESS}` in my case `ganges.usc.edu`
  - Uncomment `c.NotebookApp.port` and set it to `9999`
- Make a script called `server.sh` with the following command: `nohup jupyter server --notebook-dir='/' > server.log &`
- `./server.sh`
- `jupyter server list`
