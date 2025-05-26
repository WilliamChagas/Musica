# App de Música

Este é um app simples feito com FastAPI que serve uma música via web.  
Você pode acessar a página, ouvir a música e o código está disponível para melhorias.

## Como rodar

### 1. Clone o repositório

```bash
git clone https://github.com/WilliamChagas/Musica.git
cd Musica/main
2. Crie e ative um ambiente virtual (opcional, mas recomendado)
No Windows:

bash
Copiar
Editar
python -m venv venv
.\venv\Scripts\activate
No Linux/macOS:

bash
Copiar
Editar
python3 -m venv venv
source venv/bin/activate
3. Instale as dependências
bash
Copiar
Editar
pip install -r requirements.txt
Se você ainda não tem o arquivo requirements.txt, crie um com este conteúdo:

nginx
Copiar
Editar
fastapi
uvicorn
jinja2
4. Rode o servidor
bash
Copiar
Editar
uvicorn server:app --reload
5. Acesse no navegador
Abra o navegador e vá para:

cpp
Copiar
Editar
http://127.0.0.1:8000
6. (Opcional) Exponha seu app na internet
Para compartilhar a música com amigos, você pode usar o ngrok:

bash
Copiar
Editar
ngrok http 8000
Isso vai gerar uma URL pública para seu app.

Estrutura do projeto
csharp
Copiar
Editar
Musica/
│
├── main/
│   ├── server.py          # Código do FastAPI
│   ├── static/            # Pasta com o arquivo musica.mp3
│   └── templates/         # Pasta com index.html
│
├── requirements.txt       # Dependências Python
└── README.md              # Este arquivo
