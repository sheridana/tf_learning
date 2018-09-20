FROM python:3.6-slim

WORKDIR /tf_learning

ADD . /tf_learning

RUN pip install -r requirements.txt

RUN mkdir /notebooks && chmod a+rwx /notebooks
RUN mkdir /.local && chmod a+rwx /.local
RUN mkdir /notebooks/test
WORKDIR /notebooks
EXPOSE 8888

CMD ["bash", "-c", "source /etc/bash.bashrc && jupyter notebook --notebook-dir=/notebooks --ip 0.0.0.0 --no-browser --allow-root"]
