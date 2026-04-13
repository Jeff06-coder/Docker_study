# Define a imagem base, o que vai ser executado
FROM python:3.9-slim

# Define o diretório de trabalho dentro do container
WORKDIR /app

# Executa comandos durante a construção da imagem
RUN pip install --no-cache-dir -r requirements.txt

# Copia os arquivos do projeto para o diretório de trabalho no container
COPY . .

# Define o comando padrão ao executar o container
CMD ["python", "app.py"]