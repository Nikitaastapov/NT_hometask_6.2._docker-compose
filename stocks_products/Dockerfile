FROM python:3.9

WORKDIR /my_app

RUN pip install --upgrade pip
COPY ./my_app /my_app
RUN pip3 install --no-cache-dir --upgrade -r /my_app/requirements.txt

RUN python manage.py migrate

EXPOSE 6090

CMD ["gunicorn", "--bind", "0.0.0.0:6090", "stocks_products.wsgi"]
