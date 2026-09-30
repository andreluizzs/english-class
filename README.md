# English Class — aulas de conversação por voz com Claude

Setup de um **Projeto no Claude** para ter aulas de conversação em inglês **por áudio ao vivo**, todos os dias, com um índice de aulas e resumo de cada sessão para revisar e avançar nos temas.

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
5. **Teste da 1ª aula:** confira se, no modo voz, o Claude segue as instruções (responde curto, só em inglês, se apresenta como professor). Se não seguir, use o **ditado do teclado** no chat normal: você fala, o texto vai para o Claude, e o resto funciona igual.

## Como é uma aula (15–25 min)

| Etapa | O que você faz | O que o Claude faz |
|---|---|---|
| 1. Início | *"Let's start today's class"* | Lê o log, diz o nº da aula, aquece com o seu dia |
| 2. Conversa | Fala sobre o tema (ou propõe outro) | Respostas curtas, 1 pergunta por vez, corrige pouco |
| 3. Fechamento | *"Let's wrap up"* | Fala 3 dicas: 1 acerto, 1 erro para praticar, 1 expressão |
| 4. Resumo | Sai do modo voz e digita `Summary` | Gera o bloco da aula (temas + principais erros) |
| 5. Registro (1 min) | Cola o resumo no `03-lesson-log.md` e substitui o arquivo no projeto | Na próxima aula, retoma de onde parou |

> O Claude **não consegue salvar o arquivo sozinho** no projeto. O passo 5 é manual, mas é só copiar e colar. Sem ele, cada aula começa do zero.

## Comandos de voz

| Você diz | Efeito |
|---|---|
| *"Let's start today's class"* | Começa a aula (a 1ª é de apresentações) |
| *"Let's talk about ..."* | Muda para um tema que você escolher |
| *"Let's move on"* / *"Next topic"* | Avança para o próximo tema do roadmap |
| *"Let's review"* | Revisão dos temas anteriores e dos erros recorrentes |
| *"Let's do a call"* | Simula uma call/reunião de trabalho |
| *"Let's debate ..."* | O Claude defende o lado oposto e você argumenta |
| *"Como fala ...?"* | Recebe a palavra em inglês e a conversa **continua em inglês** |
| *"Portuguese, please"* / *"Back to English"* | Troca de idioma e volta |
| *"Let's wrap up"* | Encerra com 3 dicas faladas |
| `Summary` (digitado) | Gera o resumo da aula para o log |

## Regras de correção

| Situação | Comportamento |
|---|---|
| Erro comum | **Reformulação:** o Claude repete sua ideia do jeito certo na resposta, sem apontar o erro |
| Erro que atrapalha o sentido, que se repete ou que já está nos "Recurring mistakes" | Dica de 1 frase + *"Can you try again?"* |
| Nova tentativa | **Máximo 3 tentativas.** Se ainda errar, ele segue a conversa e anota no resumo |
| Frequência | 1 correção explícita por vez, e não a cada fala |
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

- **Consistência > duração:** 20 min todo dia rendem mais que 2h no sábado.
- **Quando travar, não mude para o português:** tente explicar com outras palavras (*"I don't know the word, but it's the thing that..."*) ou pergunte *"Como fala...?"*.
- A cada ~10 aulas, peça no chat de texto: *"Based on my lesson log, how is my progress?"*.
