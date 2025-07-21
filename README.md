🤖 Assistente de Vendas com IA - AEGia
📝 Descrição do Projeto
AEGia é um assistente de vendas inteligente, desenvolvido como um protótipo funcional para o "Teste Prático - Desenvolvimento de Projeto com IA". O objetivo do projeto é demonstrar o uso estratégico e criativo da Inteligência Artificial em um contexto de negócio real.

A aplicação funciona como um chatbot consultivo para uma empresa fictícia de cursos de marketing automotivo. A IA, nomeada "AEGia", interage com os usuários para entender seus objetivos, qualificar seu perfil e recomendar o curso mais adequado de um catálogo pré-definido.

✨ Funcionalidades Principais
Consultoria Educacional Personalizada: A IA analisa os objetivos e o perfil do usuário para recomendar o curso ideal.

Qualificação de Leads: O assistente faz perguntas estratégicas para qualificar o interesse e a necessidade do cliente.

Base de Conhecimento Própria: A IA utiliza um catálogo de cursos específico como sua única fonte de verdade, garantindo recomendações relevantes.

Redirecionamento para Vendas: Após a recomendação, o assistente fornece um link direto para a equipe de vendas no WhatsApp.

Interface de Chat Intuitiva: Construído com Streamlit para uma experiência de usuário limpa e amigável.

🛠️ Tecnologias Utilizadas

Linguagem: Python

Framework da Aplicação: Streamlit

Inteligência Artificial: Google Gemini (via API google-generativeai)

⚙️ Guia de Instalação e Execução
Para executar este projeto em seu ambiente local, siga os passos abaixo.

1. Pré-requisitos
Antes de começar, certifique-se de que você tem:

Python 3.8 ou superior instalado.

Git instalado em sua máquina.

Uma chave de API do Google AI Studio. Se não tiver uma, você pode obtê-la gratuitamente aqui.

2. Clone o Repositório
Abra seu terminal e clone este repositório para sua máquina local.

Bash

git clone https://github.com/GabrielRenanPE/AEGia.git
cd AEGia
3. Instale as Dependências
Com o ambiente virtual de sua preferência ativado, instale todas as bibliotecas necessárias com um único comando:

Bash

pip install -r requirements.txt
4. Configure sua Chave de API (Passo Crucial)
Para que a aplicação possa se conectar à IA do Google, você precisa configurar sua chave de API de forma segura usando o sistema de segredos nativo do Streamlit.

Na raiz do projeto, crie uma pasta chamada .streamlit.

Bash

mkdir .streamlit
Dentro desta nova pasta, crie um arquivo chamado secrets.toml.

Bash

# No Windows, você pode usar:
# type nul > .streamlit\secrets.toml
# No Linux/macOS, você pode usar:
# touch .streamlit/secrets.toml
Abra o arquivo .streamlit/secrets.toml e adicione sua chave de API no seguinte formato:

Ini, TOML

# Substitua o texto pela sua chave de API real
GOOGLE_API_KEY = "SUA_CHAVE_DE_API_AQUI"
Importante: O diretório .streamlit não deve ser enviado para o GitHub. O arquivo .gitignore do projeto já está configurado para ignorá-lo, garantindo a segurança de sua chave.

5. Execute a Aplicação
Com tudo configurado, inicie o servidor do Streamlit com o comando:

Bash

streamlit run appAEGia.py
