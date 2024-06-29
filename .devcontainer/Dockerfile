FROM mcr.microsoft.com/devcontainers/python:1-3.12-bullseye as base

# Install large dependencies
RUN python -m pip install --upgrade pip
RUN python -m pip install poetry jax[cpu] numpyro[cpu] 

# Install matplotlib
RUN python -m pip install matplotlib

# Install arviz
RUN apt-get update
RUN apt-get install -y libhdf5-serial-dev
RUN python -m pip install arviz

# docker run --rm your_image_name:tag
ENTRYPOINT ["/bin/bash", "python"]