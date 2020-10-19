From python:3.7-slim

ENV CONTAINER_HOME=/var/www

ADD . $CONTAINER_HOME

WORKDIR $CONTAINER_HOME

RUN pip install --no-cache-r $CONTAINER_HOME/requirements.txt

CMD ["gunicorn", "--bind",":8000", "--workers 4" "app.create_app:create_app()"]
