to run elastic search
run docker compose up

copy gemma2 at the project directory since this is where the files are located
first build the image
docker build -t ollama-gemma2b .

then run
docker run -it --rm -p 11434:11434 ollama-gemma2b

to deploy streamlit
pip install streamlit
streamlit run qa_faq.py