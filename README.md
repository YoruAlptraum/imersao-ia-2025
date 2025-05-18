# ConsultaRapida_Bot

Projeto de chatbot com Google Gemini desenvolvido para a Imersão IA da Alura.

## Descrição do Projeto

Você já se encontrou naquela situação de sentir um incômodo ou uma dor leve e não sabia se era algo sério o suficiente para procurar um médico? Muitas vezes pensamos "ainda dá pra aguentar" e acabamos apenas postergando a decisão até a situação se agravar.

Bom, o objetivo principal deste bot para Telegram é auxiliar você a tomar uma decisão mais informada sobre a necessidade de buscar atendimento médico. Através de uma conversa simples e interativa no Telegram, o bot fará perguntas relevantes sobre seus sintomas e sua condição atual. Ao final da interação, você receberá uma orientação inicial sobre se é recomendado procurar um médico o mais breve possível ou se a situação pode ser monitorada antes de tomar uma decisão.

**Importante:** Este bot oferece uma triagem inicial e **não substitui, de forma alguma, uma consulta médica profissional**. A avaliação fornecida aqui é apenas uma orientação preliminar e não deve ser considerada um diagnóstico ou recomendação de tratamento. Em caso de dúvidas persistentes ou sintomas graves, procure sempre um médico.

## Funcionalidades Principais

- **Coleta de Sintomas:** O bot será capaz de interagir com o usuário para entender seus sintomas e queixas de saúde.
- **Avaliação de Urgência:** Com base nas informações fornecidas, o bot avaliará a urgência da situação.
- **Recomendação:** O bot fornecerá uma recomendação clara ao usuário, indicando se é aconselhável procurar um médico ou se pode aguardar.
- **Indicação:** Se o bot aconselhar a produra de um médico ele oferece para buscar clinicas próximas
- **Integração com Telegram:** O bot será especificamente desenvolvido para a plataforma Telegram, aproveitando seus recursos de interação.

## Agentes

- Pesquisador: pesquisa informações dos sintomas e possiveis causas no google

retorna: possiveis causas, remediações e nível de urgência do problema (se é recomendado buscar atendimento médico ou se pode monitorar um pouco antes de tomar uma decisão)

- Mediador: simplifica a informação recebida para retornar ao usuário

retorna: informação resumida e em termos simples pede por mais informações sobre o problema se necessário, se a informação tiver boa base, identifica qual médico especialista e direciona o usuário para o médico especialista ou plantão

- Localizador: busca no google por médicos/consultórios ou pronto atendimentos próximos do usuário

retorna: médicos/consultórios ou pronto atendimentos junto a seus horários de atendimento

## Rodando o projeto

Para rodar o projeto é necessário criar um bot no Telegram usando o `@BotFather` e pegar a API Key do bot criado

No colab adicione as chaves de API do bot do Telegram e do Gemini nos secrets e depois é só rodar o bot que ja vai dar para conversar com ele
