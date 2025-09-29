from python:3.8.13 as base

ENV 

COPY 

WORKDIR 

RUN 

COPY ./ /src/

FROM base as test
RUN ["python", "-m", "pytest", "-v", "tests"]

FROM base as build
CMD streamlit run --server.port 9090 app/anyone_object_detection
