FROM python:alpine
RUN pip install flask gunicorn redis
COPY . /src
WORKDIR /src
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "--workers", "10", "counter:app"]
EXPOSE 5000
