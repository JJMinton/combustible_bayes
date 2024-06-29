FROM mcr.microsoft.com/devcontainers/python:1-3.12-bullseye as base

RUN python -m pip install --upgrade pip

# Install JAX
RUN python -m pip install jax[cpu]

# Install numpyro
RUN python -m pip install numpyro[cpu]

# docker run --rm your_image_name:tag
ENTRYPOINT ["/bin/bash", "python"]