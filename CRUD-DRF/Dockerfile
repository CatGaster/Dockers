FROM python:3.10

WORKDIR /CRUD-DRF


COPY  . .
RUN pip install -r /CRUD-DRF/requirements.txt

RUN python manage.py migrate

ENV SECRET_KEY=django-insecure-nw^y+m^wmxza1asgk+)!ua2qx9)g+#v=6%76-9i8i(6eqiw94j
RUN python manage.py migrate

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "stocks_products.wsgi"]

