FROM mcr.microsoft.com/azureml/openmpi5.0-cuda12.6-ubuntu24.04

# ONNX Runtime requires the en_US.UTF-8 locale configured.
RUN apt-get update \
    && apt-get install -y locales \
    && locale-gen en_US.UTF-8 \
    && update-locale LANG=en_US.UTF-8

ENTRYPOINT ["/opt/nvidia/nvidia_entrypoint.sh"]
