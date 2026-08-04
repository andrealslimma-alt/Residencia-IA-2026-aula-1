Criar o Ambiente Virtual (venv)
Abra seu terminal na pasta raiz do projeto ( /IA) e execute o seguinte comando para criar o ambiente virtual:
# No Linux/macOS
python3 -m venv venv
# No Windows
python -m venv venv

Sempre que para trabalhar no projeto ou rodar os códigos, você precisa ativar o venv.
# No Linux/macOS
source venv/bin/activate

# No Windows
venv\Scripts\activate

Com o ambiente ativado, instale as bibliotecas permitidas (como openaie python-dotenv) a partir do arquivo requirements.txtque está na raiz do projeto:
pip install -r requirements.txt

Para proteger seus dados e garantir a segurança, as chaves de API nunca devem ser inseridas diretamente no código nem comitadas em repositórios públicos.
-se de que o arquivo .envexiste dentro da pasta AULA_01(ou na raiz, dependendo de onde for executado) com a seguinte estrutura:
OPENAI_API_KEY=sua_chave_de_api_aqui
OPENAI_MODEL=gpt-4o-mini
(Importante: adicione o arquivo .envao seu .gitignorepara não enviá-lo para o GitHub).

Agora que o ambiente está isolado e as bibliotecas estão instaladas, você pode executar o script:
# Entre na pasta da aula
cd AULA_01

# Execute o script Python
python hello_llm.py
