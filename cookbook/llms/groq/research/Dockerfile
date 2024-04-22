FROM python:3.12.2-slim-bookworm

COPY . /app
WORKDIR /app

RUN pip install --no-cache-dir -r requirements.txt

ENV GROQ_API_KEY=""
ENV TAVILY_API_KEY=""

CMD [ "streamlit", "run", "app.py" ]
