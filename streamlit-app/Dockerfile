FROM python:3.6-slim

RUN python -m pip install --upgrade pip
RUN pip install streamlit

COPY requirements.txt .
RUN python -m pip install -r requirements.txt

COPY . .
EXPOSE 8000
CMD ["sh", "-c", "streamlit run --server.port $PORT ./my_app.py"] 