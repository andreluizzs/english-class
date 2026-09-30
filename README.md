# English Class — aulas de conversação por voz com Claude

Setup de um **Projeto no Claude** para ter aulas de conversação em inglês **por áudio ao vivo** (geralmente dirigindo), com um índice de aulas e resumo diário para revisar e avançar nos temas.

**Formato:** sessões de ~10 min, de 1 a 4 vezes por dia. **1 aula = 1 dia = 1 chat**: todas as sessões do dia acontecem no mesmo chat, e o resumo é feito uma vez só, no fim do dia.

## Arquivos

| Arquivo | Onde usar | Para quê |
|---|---|---|
| [`01-project-instructions.md`](01-project-instructions.md) | Project → **Instructions** | O "roteiro" do professor: como conversar, corrigir, conduzir e fechar a aula |
| [`02-learner-profile.md`](02-learner-profile.md) | Project → **Knowledge** | Meu nível, objetivos, contexto de trabalho, erros típicos |
| [`03-lesson-log.md`](03-lesson-log.md) | Project → **Knowledge** | Memória das aulas: status atual, roadmap de temas, erros recorrentes, índice e resumos |

## Setup (10 min)

1. No Claude: **Projects → Create project** → nome: `English Class`.
2. Em **Instructions**, cole o conteúdo de `01-project-instructions.md` (a partir da linha `# Role`).
3. Em **Knowledge**, suba `02-learner-profile.md` e `03-lesson-log.md`.
4. No app do celular, abra um novo chat **dentro do projeto**, ative o **modo voz** e diga: *"Let's start today's class"*.
5. **Faça a 1ª aula parado** (não dirigindo) e confira se, no modo voz, o Claude segue as instruções: responde curto, só em inglês, se apresenta como professor. Se não seguir, me avise para ajustarmos. O ditado do teclado segue as instruções, mas exige tocar na tela, então não serve para o carro.
6. **Opcional:** se o seu plano tiver a opção de o Claude **pesquisar e consultar conversas anteriores** (em Settings), ative. Assim ele consegue consultar as aulas anteriores do projeto além do log.

## Como é um dia de aula

| Momento | O que você faz | O que o Claude faz |
|---|---|---|
| **1ª sessão** (novo chat) | *"Let's start today's class"* | Lê o log, diz o nº da aula, 1 pergunta de aquecimento, entra no tema |
| **Durante** (~10 min) | Conversa sobre o tema (ou propõe outro) | Respostas curtas, 1 pergunta por vez, no máx. 2 correções por sessão |
| **Fim da sessão** | *"Let's wrap up"* ou *"I have to go"* | 2 frases: 1 erro para praticar + 1 expressão |
| **Próximas sessões** (mesmo chat) | *"I'm back"* / *"Let's continue"* | Retoma o tema e traz de volta o erro da sessão anterior |
| **Fim do dia** (parado) | Digita `Summary` | Gera o resumo do dia inteiro (temas + principais erros) |
| **Registro** (1 min) | Cola o resumo no `03-lesson-log.md` e substitui o arquivo no projeto | Na próxima aula, retoma de onde parou |

> O Claude **não consegue salvar o arquivo sozinho** no projeto. O registro é manual (copiar e colar, 1x por dia). Sem ele, cada aula começa do zero.

## No carro

- **Prepare antes de sair:** abra o app, entre no projeto (ou no chat do dia) e ative o modo voz **com o carro parado**. Depois disso, é só falar.
- O Claude está instruído a **nunca pedir para você ler, digitar ou olhar a tela** durante a sessão.
- Se a sessão cair ou você chegar no destino no meio da conversa, sem problema: na próxima, diga *"I'm back"* no mesmo chat.
- `Summary` e o registro no log ficam para quando estiver parado.

## Comandos de voz

| Você diz | Efeito |
|---|---|
| *"Let's start today's class"* | Começa a aula do dia em um chat novo (a 1ª é de apresentações) |
| *"I'm back"* / *"Let's continue"* | Nova sessão no mesmo chat do dia |
| *"Let's talk about ..."* | Muda para um tema que você escolher |
| *"Let's move on"* / *"Next topic"* | Avança para o próximo tema do roadmap |
| *"Let's review"* | Revisão dos temas anteriores e dos erros recorrentes |
| *"Let's do a call"* | Simula uma call/reunião de trabalho |
| *"Let's debate ..."* | O Claude defende o lado oposto e você argumenta |
| *"Como fala ...?"* | Recebe a palavra em inglês e a conversa **continua em inglês** |
| *"Portuguese, please"* / *"Back to English"* | Troca de idioma e volta |
| *"Let's wrap up"* / *"I have to go"* | Encerra a sessão com 2 dicas faladas |
| `Summary` (digitado, fim do dia) | Gera o resumo do dia para o log |

## Regras de correção

| Situação | Comportamento |
|---|---|
| Erro comum | **Reformulação:** o Claude repete sua ideia do jeito certo na resposta, sem apontar o erro |
| Erro que atrapalha o sentido, que se repete ou que já está nos "Recurring mistakes" | Dica de 1 frase + *"Can you try again?"* |
| Nova tentativa | **Máximo 3 tentativas.** Se ainda errar, ele segue a conversa e anota no resumo |
| Frequência | 1 correção explícita por vez, **no máximo 2 por sessão** |
| Pronúncia / sotaque | Não é avaliada (o áudio vira texto antes de chegar ao Claude) |

## Evolução dos temas

- O **roadmap** fica no `03-lesson-log.md`: Introductions → Daily routine → Free time → Series & movies → Food & travel → Sports → Personal finance → Work → Meetings & calls → Debate → Free topics.
- Um tema pode durar várias aulas. O Claude **só avança quando você pedir**; se perceber que você está confortável, ele sugere, mas pergunta antes.
- Você pode editar o roadmap à vontade: reordenar, incluir ou remover temas.
- Quando quiser consolidar, peça *"Let's review"*: ele usa os resumos e os erros recorrentes do log.

## Sobre o meu nível (certificado vs. percepção)

O laudo do curso confirma a percepção de estar um nível abaixo na fala:

- Notas de 88–89% em comunicação, interação e segurança → **compreende e se vira bem** (B2 para ouvir e ler).
- Mas também: *"tende à simplificação"*, *"comete erros em estruturas mais avançadas"*, *"busca por palavras"*, *"dificuldade em debate"*, *"hesita no uso informal"*.
- E: *"alto conhecimento gramatical"* → **sabe a regra, mas ela ainda não sai automática na fala.**

Por isso o foco é **volume de conversa por voz**, com correção leve e retomada dos erros recorrentes, em vez de mais gramática.

## Dicas

- **Consistência > duração:** várias sessões curtas por dia rendem mais que 2h no sábado.
- **Quando travar, não mude para o português:** tente explicar com outras palavras (*"I don't know the word, but it's the thing that..."*) ou pergunte *"Como fala...?"*.
- A cada ~10 aulas (dias), peça no chat de texto: *"Based on my lesson log, how is my progress?"*.
