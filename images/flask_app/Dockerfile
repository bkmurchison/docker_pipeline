FROM python:3.14.3-slim-trixie
RUN useradd -m -s /bin/bash appuser
WORKDIR /app
COPY src/* ./
RUN pip install --no-cache-dir -r requirements.txt
USER appuser
CMD ["python", "app.py"]
