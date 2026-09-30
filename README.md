# English Class — prática diária de conversação com Claude

Setup de um **Projeto no Claude** para praticar conversação todos os dias, calibrado para o meu nível real (B2 no certificado, B1+ na fala).

## Arquivos

| Arquivo | Onde usar | Para quê |
|---|---|---|
| [`01-project-instructions.md`](01-project-instructions.md) | Project → **Instructions** | O "prompt" do professor: regras, correções, modos, feedback |
| [`02-learner-profile.md`](02-learner-profile.md) | Project → **Knowledge** | Meu nível, objetivos, contexto de trabalho, erros típicos |
| [`03-progress-log.md`](03-progress-log.md) | Project → **Knowledge** | Memória entre sessões: erros recorrentes e foco da semana |

## Setup (10 min)

1. No Claude: **Projects → Create project** → nome: `English Coach`.
2. Em **Instructions**, cole o conteúdo de `01-project-instructions.md` (a partir da linha `# Role`).
3. Em **Knowledge**, suba `02-learner-profile.md` e `03-progress-log.md`.
4. Abra um chat no projeto e digite: `level check`.
5. Cole o bloco de log do resultado em `03-progress-log.md` e reenvie o arquivo.

## Rotina diária (20–25 min)

| Etapa | Tempo | Como |
|---|---|---|
| 1. Abrir | 1 min | Novo chat no projeto → `start` (ou a palavra do modo) |
| 2. Falar | 15 min | **Voz ou ditado do teclado** — não digite (ver abaixo) |
| 3. Feedback | 3 min | `end` → ler os 5 erros e as 5 expressões **em voz alta** |
| 4. Registrar | 1 min | Copiar o bloco de log para o `03-progress-log.md` |

**Semana:** Seg `work` · Ter `smalltalk` · Qua `call` · Qui `debate` · Sex `retell` + revisão · Fim de semana `daily` (opcional).

**Sexta (revisão semanal, +5 min):** atualizar "Current focus" e "Recurring mistakes" no log e reenviar o arquivo no projeto.

## Palavras-chave durante o chat

| Digite | Efeito |
|---|---|
| `work` / `call` / `debate` / `smalltalk` / `daily` / `retell` | Muda o modo da sessão |
| `grammar present perfect` | Mini-treino de uma estrutura (5 exercícios) + uso na conversa |
| `voice` | Para de corrigir a cada turno; junta tudo no final |
| `help` | Recebe 2–3 começos de frase (não a resposta pronta) |
| `PT?` | Explicação em português |
| `end` | Feedback final + bloco de log |
| `level check` | Teste de nivelamento (refazer 1x por mês) |

## Análise crítica do prompt original

O prompt de exemplo é um bom ponto de partida, mas tem lacunas que fazem a prática render menos:

| Ponto | Problema | Ajuste feito |
|---|---|---|
| **Só texto** | Digitar não é conversar. Você tem tempo de pensar, consultar, reescrever — o oposto de uma reunião. | Prioridade para **voz / ditado**. Texto fica para `grammar` e revisão. |
| **Corrigir todo erro** | Sobrecarga: 6 correções por resposta = você não retém nenhuma e perde o ritmo. | **Máx. 3 por turno**, priorizando erros que mudam o sentido e erros recorrentes. |
| **Corrigir no modo voz** | Interromper a cada fala quebra a fluência — que é justamente o seu ponto fraco. | No modo voz, correções só no final (`end`). |
| **Idiom sempre** | Idioms são pouco usados em reunião de trabalho; decorar "raining cats and dogs" não ajuda. | Foco em **collocations e phrasal verbs** ("follow up", "roll out", "sort out"). |
| **Nível genérico** ("intermediário") | O Claude não sabe *onde* você trava. | Perfil com os pontos fracos do laudo do curso + erros típicos de brasileiro. |
| **Sem memória** | Cada chat começa do zero; os mesmos erros voltam sem ninguém perceber. | `03-progress-log.md` + marcação `🔁 Again!` para erro repetido. |
| **IA fala demais** | Chatbot tende a responder com parágrafos; quem precisa falar é você. | Resposta curta (~60 palavras) e **obriga a expandir** respostas curtas. |
| **Tema aleatório** | Pouca transferência para o seu dia a dia real. | Modos `work`, `call` e `debate` com cenários de produto, integração bancária e negociação. |

## Sobre o seu nível (certificado vs. percepção)

Sua percepção faz sentido, e o próprio laudo do curso confirma:

- Notas de 88–89% em comunicação, interação e segurança → você **compreende e se vira bem** (B2 receptivo).
- Mas o texto também diz: *"tende à simplificação"*, *"comete erros em estruturas mais avançadas"*, *"busca por palavras"*, *"dificuldade em debate ou confronto de ideias"*, *"hesita no uso informal"*.
- E um ponto importante: *"alto conhecimento gramatical"*. Ou seja, **você sabe a regra, mas ela ainda não sai automática na fala.**

**Conclusão:** o problema não é falta de conteúdo, é **automatização**. Por isso o setup força volume de fala, repetição dos mesmos erros até sumirem, e cenários parecidos com a vida real. Estudar mais gramática em texto não resolve esse gap.

## Dicas práticas

- **Ditado do teclado** (microfone do teclado do celular) é o melhor dos dois mundos: você **fala**, mas o Claude recebe texto e consegue corrigir. Use quando quiser correção turno a turno.
- **Modo voz do app** (se disponível dentro do projeto): use no `call` e no `smalltalk`, para treinar ritmo e compreensão.
- **Não troque para o português** quando travar: use `help` ou parafraseie ("I don't know the word, but it's the thing that...") — é exatamente essa habilidade que o `call` treina.
- **Refaça o `level check` todo mês** e compare as notas no log.
- **Consistência > duração:** 20 min todo dia rendem mais que 2h no sábado.
