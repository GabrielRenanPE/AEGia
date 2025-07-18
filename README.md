# 🤖 Assistente de Vendas com IA - AEGia

## 📝 Descrição do Projeto

**AEGia** é um assistente de vendas inteligente, desenvolvido como um protótipo funcional para o "Teste Prático - Desenvolvimento de Projeto com IA". O objetivo do projeto é demonstrar o uso estratégico e criativo da Inteligência Artificial em um contexto de negócio real.

A aplicação funciona como um chatbot consultivo para uma empresa fictícia de cursos de marketing automotivo. A IA, nomeada "AEGia", interage com os usuários para entender seus objetivos, qualificar seu perfil e recomendar o curso mais adequado de um catálogo pré-definido.

## ✨ Funcionalidades Principais

  * [cite\_start]**Consultoria Educacional Personalizada:** A IA analisa os objetivos e o perfil do usuário para recomendar o curso ideal[cite: 1].
  * [cite\_start]**Qualificação de Leads:** O assistente faz perguntas estratégicas para qualificar o interesse e a necessidade do cliente antes de fazer uma recomendação[cite: 1].
  * [cite\_start]**Base de Conhecimento Própria:** A IA utiliza um catálogo de cursos específico como sua única fonte de verdade, garantindo que as recomendações sejam sempre relevantes para o negócio[cite:1].
  * [cite\_start]**Redirecionamento para Vendas:** Após a recomendação e o interesse do usuário, o assistente fornece um link direto para a equipe de vendas no WhatsApp, finalizando o processo de qualificação[cite: 1].
  * **Interface de Chat Intuitiva:** Construído com Streamlit, o projeto oferece uma experiência de usuário limpa e amigável.

## 🛠️ Tecnologias Utilizadas

  * **Linguagem:** Python
  * **Framework da Aplicação:** Streamlit
  * **Inteligência Artificial:** Google Gemini (via API `google-generativeai`)

## ⚙️ Instalação e Configuração

Para executar este projeto localmente, siga os passos abaixo.

### 1\. Pré-requisitos

  - Python 3.8 ou superior
  - Uma chave de API do [Google AI Studio](https://aistudio.google.com/app/apikey)

### 2\. Clone o Repositório

```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
```

### 3\. Instale as Dependências

```bash
pip install -r requirements.txt
```

*Obs: Se não houver um arquivo `requirements.txt`, você pode instalar as bibliotecas manualmente:*

```bash
pip install streamlit google-generativeai
```

### 4\. Configure sua Chave de API

Por segurança, o projeto utiliza o sistema de segredos do Streamlit.

1.  Crie uma pasta na raiz do projeto chamada `.streamlit`.

2.  Dentro desta pasta, crie um arquivo chamado `secrets.toml`.

3.  Adicione sua chave de API do Google ao arquivo da seguinte forma:

    ```toml
    # .streamlit/secrets.toml
    GOOGLE_API_KEY = "SUA_CHAVE_API_AQUI"
    ```

## 🚀 Como Executar

Com as dependências instaladas e a chave de API configurada, execute o seguinte comando no seu terminal:

```bash
streamlit run appAEGia.py
```

A aplicação será aberta automaticamente no seu navegador padrão.

-----
