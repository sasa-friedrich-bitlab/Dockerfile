
FROM ubuntu:20.04
LABEL maintainer="Saša Friedrich <sasa.friedrich@bitlab.si>"

RUN apt-get update && apt-get install -y \
    openssh-client \
    ansible \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /ansible

ENTRYPOINT ["ansible-playbook"]
CMD ["--help"]
