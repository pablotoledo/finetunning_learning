FROM jupyter/base-notebook

# Dependencies
RUN pip install numpy pandas scipy scikit-learn matplotlib
USER root
RUN echo "jovyan ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/jovyan && \
    chmod 0440 /etc/sudoers.d/jovyan
USER jovyan

# Configura el directorio de trabajo
WORKDIR /home/notebook

