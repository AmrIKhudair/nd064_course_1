FROM python:2.7
EXPOSE 7111
WORKDIR /app
COPY techtrends/requirements.txt ./requirements.txt
RUN pip install -r requirements.txt
COPY techtrends .
RUN python init_db.py
CMD [ "python", "app.py" ]