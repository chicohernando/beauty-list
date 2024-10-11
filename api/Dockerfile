FROM python:3.10

WORKDIR /srv/beauty-list/api

COPY ./requirements.txt .

RUN pip install --upgrade pip
RUN pip install --no-cache-dir --upgrade -r /srv/beauty-list/api/requirements.txt

EXPOSE 80

CMD ["fastapi", "run", "app/main.py", "--reload", "--port", "80"]