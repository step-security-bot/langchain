FROM python:3.9@sha256:70dce00379744edb10d8c7ee8339bbf964dcbcadc1da862bdc59dc746513c04c

RUN pip install httpx PyGithub "pydantic==2.0.2" pydantic-settings "pyyaml>=5.3.1,<6.0.0"

COPY ./app /app

CMD ["python", "/app/main.py"]