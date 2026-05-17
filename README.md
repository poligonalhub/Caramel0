## Caram3l0, melhor amigo de artista que sofre com editais.
![Caram3l0V1](/assets/caramelov1.png)

---

## **O QUE É O** `Caram3l0`**?**

- **Procura editais culturais** em vários sites, nacionais e nordestinos.
- Ao encontrar um edital, ele **dá uma olhada** para ver se tem o link para o documento (tipo um PDF), se tem prazo para se inscrever e se diz quais áreas podem participar.
- Se o edital estiver "completo" com essas informações, ele **guarda** isso em um lugar seguro.
- Depois, ele **avisa** sobre o edital novo que ele encontrou e **manda lembretes importantes** antes do prazo final, tipo "Última semana!" ou "Último dia!".

Basicamente, ele é feito para encontrar e disparar atualizações sobre oportunidades de patrocínio e financiamento para projetos culturais, focando em algumas regiões específicas.

## COMO FUNCIONA?

- A cada hora, `Caram3l0` busca novos editais em vários sites cadastrados, procurando termos relevantes como “edital”, “chamada pública”, “oportunidade”, “patrocínio”, “seleção”, “incentivo” e outras palavras-chave relativas à fontes de financiamento.
- Extrai informações essenciais de potenciais editais encontrados.
- Valida cada edital verificando a presença de:
    - **Link direto para o documento oficial** (.PDF, .DOCX, .DOC, .CVS, .PPTX, .PPT).
    - **Prazo de inscrição**.
    - **Categorias participantes**.
    - Valores totais e por categorias / projetos.
- Descarta editais que não contenham as informações essenciais validadas.
- Armazena editais validados.
- Posta avisos no Discord ao encontrar um novo edital validado ('EDITAL ABERTO').
- Configura lembretes e os envia ('ÚLTIMA SEMANA DE INSCRIÇÕES' e 'ÚLTIMO DIA') conforme os prazos se aproximam.
- Prioriza busca por editais com ênfase em João Pessoa, na Paraíba, e na região Norte-Nordeste do Brasil.

---

ETAPA5

1) **FAREJANDO** *coleta de dados

Uma vez/hora Caram3l0 raspa dados de seu POTE DE RAÇÃO (desde oportunidades nacionais, até entes locais como FUNJOPE e JPCultural) procurando por arquivos e palavras-chaves comuns ("editais", "patrocínio", "seleção", "regulamento", "chamada pública", "inscrições abertas", "lei de fomento", etc) em anúncios de oportunidades de financiamento.

2) **RABO LEVANTADO** *validação

Ao se deparar com uma possível oportunidade, `Caram3l0` verifica

2.1. **SE** esse edital já está no POTE. **SE SIM**, Caram3l0 bate a data pra checar se é uma prorrogação. **SE FOR**, `Caram3l0` dispara o latido de prorrogação; **SE NÃO** for prorrogação, `Caram3l0` descansa (2.1.1. **RABO ABAIXADO** **Assync/Await*) até voltar pra primeira etapa na próxima hora. **SE NÃO** estiver no banco, ele continua fuçando para checar

2.2. **SE** há um link de download direto para o arquivo do edital (.PDF, DOCX, .DOC, .PPT, PPTX, HTML, .CSV, RTF, PLAIN, .TXT, etc).

2.3. **SE** o edital já expirou (se não tiver mais fonte disponível, `Caram3l0` descansa (2.1.1. **RABO ABAIXADO**).

2.4. **SE** o plano de ação (cronograma) do edital e seus valores (orçamento total e por projeto) foram discriminados.

2.5. **SE** está explícito quais áreas e categorias serão contempladas.

Caso o edital raspado seja novo (não esteja no banco de dados e está em andamento) e passe pelos critérios de validação, ele é salvo no POTE com uma ID única, evitando duplicações e preparando o terreno para caso o edital prorrogue. Além da ID única, junto com o arquivo do edital são salvos também suas informações mais relevantes (datas, cronogramas, orçamentos, vigência, fonte, etc) para acesso rápido no POTE.

3) **POTE DE RAÇÃO** *banco de dados

Com uma nova entrada validada, podemos raspar mais informações detalhadas sobre finalidade, categorias, prazos, público-alvo, se é PF, PJ (MEI ou produtora) e outras peculiaridades de cada edital. Pra garantir uma captura confiável e que leve em consideração a estrutura de cada site, os raspadores (scrapers) partem do mesmo template, mas se diferem para contemplar cada fonte distinta, cada uma com um raspador separado (um arquivo .js independente). Isso facilita a manutenção caso algum site atualize sua estrutura, evitando que a lógica geral quebre, inutilizando apenas a raspagem do site modificado em questão. 

P0TE INICIAL:

Caixa Cultural - Seleção
https://www.selecaocaixacultural.com.br/?utm_source=google&utm_medium=search&utm_campaign=cultural_edital_2025&utm_term=cc0651&utm_content=cc0651&gad_source=1&gad_campaignid=22531712145&gbraid=0AAAAAounJoKFO7uREFi-4RH1uLYlUPus1&gclid=Cj0KCQjwxdXBBhDEARIsAAUkP6hByRZ0MgyL5yT-KwZwAb5hyia3EdalGUxKASsfHLiZdAVBak9A8MMaAmhvEALw_wcB

Ministério da Cultura - Editais Abertos
https://www.gov.br/cultura/pt-br/assuntos/editais/inscricoes-abertas

PROSAS - Plataforma de Editais
https://prosas.com.br/editais

Mapa da Cultura – Oportunidades
https://mapa.cultura.gov.br/oportunidades/

Funjope – Fundação Cultural de João Pessoa
https://www.joaopessoa.pb.gov.br/secretarias/funjope/

Secretaria de Estado da Cultura da Paraíba (SECULT-PB)
https://www.paraiba.pb.gov.br/diretas/secretaria-da-cultura

JP Cultura – Oportunidades
https://jpcultura.joaopessoa.pb.gov.br/oportunidades/

Prefeitura de João Pessoa – Notícias
https://www.joaopessoa.pb.gov.br/categoria/noticias/

4) **LATIDO5** - Agitação e Propagação

Com editais filtrados, validados e armazenados, é hora de mostrá-los! Assim que um edital concluir sua etapa de raspagem, Caram3l0 ira formatar as informações capturadas e as distribuirá para o canal do Discord, no Whatsapp e no SITE do app

T3CH STACK
JavaScript

[Node.js](https://nodejs.org/pt/learn/getting-started/introduction-to-nodejs)

[Puppeteer](https://pptr.dev/)

[Cheerios](https://cheerio.js.org/)

[get-urls](https://www.npmjs.com/package/get-urls)

[node-fetch](https://www.npmjs.com/package/node-fetch)

[Cross-Origin Resource Sharing (CORS)](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Guides/CORS)

[IndexedDB](https://developer.mozilla.org/pt-BR/docs/Web/API/IndexedDB_API)
