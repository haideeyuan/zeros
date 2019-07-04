FROM python:3.6-slim
ADD ./mlpipeline-ui-metadata.json /
RUN mkdir -p /app
ENV APP_HOME /app
COPY ./validate.py $APP_HOME
WORKDIR $APP_HOME
ENTRYPOINT ["python", "validate.py"]
