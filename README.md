# test_doc_rag

Execute this commands to set an run `ollama`:

```bash
mkdir ollama_files

docker run -it \
    --rm \
    -v ./ollama_files:/root/.ollama \
    -p 11434:11434 \
    --name ollama \
    ollama/ollama
```

Then set the `virtualenv`

```bash
python -m venv .venv
```

After that pull the `ollama` model `llama3` of `8b` connecting to the docker container 

```bash
docker exec -it ollama bas
ollama pull llama3:8b
```
