# Groq Researcher

> Note: Fork and clone this repository if needed

### 1. Create a virtual environment

```shell
python3 -m venv ~/.venvs/aienv
source ~/.venvs/aienv/bin/activate
```

### 2. Export your Groq & Tavily API Key

```shell
export GROQ_API_KEY=***
export TAVILY_API_KEY=sk-***
```

### 3. Install libraries

```shell
pip install -r cookbook/llms/groq/research/requirements.txt
```

### 4. Run Streamlit App

```shell
streamlit run cookbook/llms/groq/research/app.py
```

- Open [localhost:8501](http://localhost:8501) to view your Groq Researcher.

### 5. Message on [discord](https://discord.gg/4MtYHHrgA8) if you have any questions

### 6. Star ⭐️ the project if you like it.

### 7. Run with Docker

```shell
# Optionally Build the image
docker build -t valeriusm/phidata-groq-research:latest .
# Run the image
docker run -d --name=phidata-groq \
      --restart=unless-stopped \
      -p 8501:8501 \
      -e GROQ_API_KEY=<your api key> -e TAVILY_API_KEY=<your api key> \
      valeriusm/phidata-groq-research:latest
```
