FROM jupyter/minimal-notebook

# Install Redis dependencies
USER root
RUN apt-get update && apt-get install -y \
        build-essential


# Install Redis module using pip
RUN pip install redis

# Set working directory
WORKDIR /home/ubuntu/Jupyter_redis/work

# expose port
EXPOSE 8080

# Start Jupyter Notebook
CMD ["jupyter"]
