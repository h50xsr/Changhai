FROM python

WORKDIR /user/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 6000

CMD ["flask", "--app", "ltitool", "run", "--host", "0.0.0.0", "--port", "6000"]
