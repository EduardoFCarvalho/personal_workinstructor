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

## ✨ Como Colocar Essa Mágica Para Rodar?

Para fazer a orquestra de agentes tocar, você vai precisar de algumas coisinhas e seguir uns passinhos:

1.  **Pré-requisitos:**
    * **Python:** Obviamente! (Versão 3.7+ é recomendada).
    * **Bibliotecas Essenciais:** Você precisa das bibliotecas `google-genai` e `google-adk`. Instale-as usando pip:
        ```bash
        pip install google-genai google-adk
        ```
    * **Sua Chave Secreta do Google Gemini:** Este projeto usa a API do Google Gemini. Você precisa obter uma chave API no Google AI Studio ([https://aistudio.google.com/](https://aistudio.google.com/)) ou na Google Cloud Platform.

2.  **Configurando sua Chave API:**
    O código no exemplo usa `google.colab.userdata.get('GOOGLE_API_KEY')`, que é comum no Google Colab. Para rodar localmente ou em outro ambiente, você precisará definir a variável de ambiente `GOOGLE_API_KEY` com sua chave. Exemplo (no Linux/macOS):
    ```bash
    export GOOGLE_API_KEY='SUA_CHAVE_AQUI'
    ```
    Ou no Windows (CMD):
    ```cmd
    set GOOGLE_API_KEY=SUA_CHAVE_AQUI
    ```
    Ou diretamente no seu script (apenas para testes locais, não recomendado para produção ou commits):
    ```python
    os.environ["GOOGLE_API_KEY"] = "SUA_CHAVE_AQUI"
    ```
    **⚠️ Mantenha sua chave API segura! Não a exponha publicamente.**

3.  **Rodando o Script:**
    Salve o código fornecido em um arquivo Python (ex: `assistente_emprego.py`) e execute-o pelo terminal:
    ```bash
    python assistente_emprego.py
    ```

4.  **Interagindo com o Assistente:**
    O assistente vai iniciar uma conversa e te fazer algumas perguntas. Responda com calma e o máximo de detalhes que se sentir confortável, especialmente sobre a descrição da vaga!

    * `Qual sua idade?`
    * `Qual cargo você vai atuar?`
    * `Em quanto tempo você vai iniciar as atividades?`
    * `Descreva seus conhecimentos atuais com relação as informações da vaga:`
    * `Descreva a vaga que você vai atuar:`

    **Para sair a qualquer momento, basta digitar `exit`.**

5.  **Aguardando a Mágica Acontecer:**
    Depois de coletar suas informações, a orquestra de agentes entrará em ação. Você verá algumas mensagens indicando que os agentes estão trabalhando. Relaxe, tome um café (ou o que preferir!) e espere o resultado.

## 🎉 O Resultado Final!

Ao final do processo, você receberá o **plano de estudos sugerido pelo Agente Estrategista**, com tópicos e links para cursos online relevantes que podem te ajudar a se preparar para os desafios do seu novo cargo!

Espero que este assistente te ajude a começar com o pé direito!

## 🤝 Quer Ajudar a Melhorar?

Este é apenas o começo! Ideias para novos agentes (ex: um que simule entrevistas?), melhorias na orquestração ou qualquer outra contribuição são super bem-vindas! Sinta-se à vontade para abrir Issues ou enviar Pull Requests.

**Boa sorte na sua nova jornada profissional!** 💪✨
