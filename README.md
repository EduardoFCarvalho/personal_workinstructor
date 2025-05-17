# 🚀 Seu Assistente Pessoal para Arrasar no Novo Emprego! ✨

Cansado de sentir aquele friozinho na barriga antes de começar um emprego novo? Que tal ter um assistente super inteligente para te dar uma mãozinha e te ajudar a chegar preparado(a)?

Este projeto é um **chatbot divertido em Python**, construído com a magia do Google Gemini e do Framework ADK (Agent Development Kit), pronto para te ajudar a entender seu novo desafio e se preparar com tudo!

## 🤔 Qual a Finalidade Disso Tudo?

A ideia é simples, mas poderosa: coletar algumas informações sobre você (seu perfil, experiência) e sobre a vaga dos seus sonhos (ou a que você acabou de conquistar!). Com isso, nossos agentes especializados entram em ação para:

1.  **Entender Quem Você É:** Analisar seu perfil e conhecimentos atuais.
2.  **Decifrar a Vaga:** Quebrar a descrição da vaga em tópicos, buscando informações quentes e atuais na internet.
3.  **Montar um Plano de Batalha:** Criar um cronograma de estudos ninja e encontrar cursos online relevantes para você chegar chegando!

Tudo isso de forma **positiva e encorajadora**!

## 🤖 A Orquestra de Agentes Mágicos

Nosso assistente funciona como uma verdadeira orquestra, onde cada "Agente" tem uma função super importante, coordenada pelo nosso "Maestro":

* 🤖 **Agente Identificador:** O detetive do grupo! Analisa sua idade, cargo e conhecimentos prévios para traçar um perfil inicial de quem você é nesse novo contexto profissional.
* 🔍 **Agente Interpretador:** O especialista em vagas! Pega a descrição do seu futuro emprego, usa a busca do Google (`Google Search`) para encontrar informações atuais sobre os temas da vaga e te entrega os pontos chave mastigadinhos, tópico a tópico.
* 🧠 **Agente Estrategista:** O guru dos estudos! Este é o cara (ou agente)! Usando seu perfil, o prazo que você tem para começar e as informações detalhadas da vaga (fornecidas pelo Agente Interpretador), ele planeja um cronograma de estudos personalizado e busca cursos online relevantes (`Google Search`) para te dar aquele empurrãozinho.
* 🎶 **Agente Orquestrador:** O maestro! Ele não gera conteúdo final diretamente, mas é quem coordena toda essa sinfonia! Ele recebe suas informações, as distribui para os agentes certos na sequência correta (Identificador -> Interpretador -> Estrategista) e garante que a resposta final (o plano de estudos!) chegue até você.

## ✨ Como Colocar Essa Mágica Para Rodar (no Google Colab)?

Este projeto foi pensado para brilhar diretamente no Google Colab! É rápido, fácil e você não precisa configurar quase nada na sua máquina.

Para fazer a orquestra de agentes tocar, siga estes passinhos:

1.  **Abrindo no Google Colab:**
    * Clique no botão Open in Colab.
       ou.
    * Copie todo o código do projeto.
    * Abra um novo Notebook no Google Colab ([https://colab.research.google.com/](https://colab.research.google.com/)).
    * Cole o código na primeira célula.

2.  **Pré-requisitos Mágicos:**
    * **Python:** O Colab já vem com Python instalado. Menos uma coisa pra se preocupar! 😉
    * **Bibliotecas Essenciais:** Você precisa das bibliotecas `google-genai` e `google-adk`. As primeiras linhas do código já incluem os comandos para instalá-las direto no ambiente do Colab:
        ```python
        !pip install google-genai
        !pip install -q google-adk
        ```
        Estas linhas serão executadas quando você rodar a primeira célula.
    * **Sua Chave Secreta do Google Gemini:** Este projeto usa a API do Google Gemini. Você precisa obter uma chave API no Google AI Studio ([https://aistudio.google.com/](https://aistudio.google.com/)) ou na Google Cloud Platform. No Colab, a forma mais segura de usar é através da ferramenta `userdata`:
        * No menu lateral esquerdo do Colab, clique no ícone da **chave (🔒)**.
        * Clique em **"+ Adicionar um novo secret"**.
        * No campo "Name", digite `GOOGLE_API_KEY`.
        * No campo "Value", cole a sua chave API do Google Gemini.
        * Marque a opção "Notebook access" para habilitar o acesso a essa chave no seu notebook.
        * O código `os.environ["GOOGLE_API_KEY"] = userdata.get('GOOGLE_API_KEY')` já está pronto para buscar a chave que você salvou nos secrets do Colab.

3.  **Rodando o Script no Colab:**
    * Com o código colado e a chave API salva nos Secrets (passo 2), basta rodar as células do notebook sequencialmente.
    * A primeira célula instalará as bibliotecas e configurará a API Key.
    * As células seguintes definirão as funções e a lógica principal.
    * A parte final do script (`if __name__ == "__main__":`) iniciará a interação.

4.  **Interagindo com o Assistente:**
    A execução vai parar e pedir sua interação nas células de input. Responda com calma e o máximo de detalhes que se sentir confortável quando o assistente perguntar:

    * `Qual sua idade?`
    * `Qual cargo você vai atuar?`
    * `Em quanto tempo você vai iniciar as atividades?`
    * `Descreva seus conhecimentos atuais com relação as informações da vaga:`
    * `Descreva a vaga que você vai atuar:`

    **Para sair a qualquer momento, basta digitar `exit` na caixa de input e apertar Enter.**

5.  **Aguardando a Mágica Acontecer:**
    Depois de coletar suas informações, a orquestra de agentes entrará em ação. Você verá mensagens indicando que os agentes estão trabalhando e, eventualmente, as respostas intermediárias do Identificador e Interpretador. Relaxe, tome um café (ou o que preferir!) e espere o resultado final do Estrategista aparecer.

## 🎉 O Resultado Final!

Ao final do processo, você receberá o **plano de estudos sugerido pelo Agente Estrategista**, com tópicos e links para cursos online relevantes que podem te ajudar a se preparar para os desafios do seu novo cargo!

Espero que este assistente te ajude a começar com o pé direito!


**Boa sorte na sua nova jornada profissional!** 💪✨
