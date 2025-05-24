FROM python:3

WORKDIR /PhisherMan

COPY . /PhisherMan

RUN apt-get update && \
    apt-get install -y php openssh-client && \
    apt-get clean

RUN pip install --no-cache-dir -r files/requirements.txt

CMD ["python3", "phisherman.py", "--noupdate"]
