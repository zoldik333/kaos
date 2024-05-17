FROM python:3
WORKDIR /poll
COPY requirements.txt ./
RUN pip3 install --no-cache-dir -r requirements.txt
COPY . .
EXPOSE 80
CMD [ "python", "-B", "./app.py" ]
