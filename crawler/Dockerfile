FROM --platform=linux/amd64 python:3.8-slim
RUN mkdir src
WORKDIR src/
COPY ../../crawler .
RUN pip install jupyter ipykernel numpy matplotlib pandas bs4 requests pymongo
CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]