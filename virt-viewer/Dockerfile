FROM debian:sid-slim
LABEL maintainer="Saša Friedrich <sasa.friedrich@bitlab.si>"

RUN apt-get update && apt-get install -y \
	libgl1-mesa-dri \
	libgl1-mesa-glx \
    openssh-client \
	virt-viewer \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["virt-viewer"]
CMD ["--help"]