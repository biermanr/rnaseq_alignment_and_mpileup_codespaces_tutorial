FROM condaforge/mambaforge:latest

# Copy environment file
COPY environment.yml /tmp/environment.yml

# Create the conda environment
RUN mamba env create -f /tmp/environment.yml && \
    mamba clean -afy && \
    rm /tmp/environment.yml

# Configure bash to activate the environment by default
RUN echo 'conda activate rnaseq' >> /root/.bashrc

# Set working directory
WORKDIR /workspaces

# The environment is now pre-built and ready to use
