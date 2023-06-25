FROM jupyter/minimal-notebook

USER root

# Install Redis dependencies
RUN apt-get update && \
    apt-get install -y \
        build-essential \
        tcl

USER $NB_UID

# Install Redis module using pip
RUN pip install redis

# Start Jupyter Notebook
CMD ["start-notebook.sh"]
