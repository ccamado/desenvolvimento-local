# Central de Avisos - 2o Ano IA

## Turma e itinerario

- Turma: 2o ano do Ensino Medio.
- Itinerario formativo profissional: Inteligencia Artificial.
- Qualificacao: Desenvolvedor de Algoritmos de Aprendizado de Maquina.
- Projeto ancora: Central de Avisos.

## Objetivo do sistema

Criar uma pagina de chat onde o usuario digita perguntas sobre horarios, provas, trabalhos, eventos e comunicados da escola. O sistema deve consultar dados reais em uma planilha MASTER e devolver respostas organizadas, sem inventar informacao.

## Solucao tecnica prevista

- Google Sheets.
- Google Apps Script.
- Web App em formato de chat.
- Sem custo financeiro.

## Planilha MASTER

### Aba HORARIO_SEMANAL

- Turma
- DiaSemana
- Tempo
- Inicio
- Fim
- Disciplina
- Professor

### Aba AVISOS

- ID
- DataCadastro
- Turma
- Tipo
- Disciplina
- DataDoEvento
- Hora
- MensagemCurta
- Responsavel
- Validade

Tipos definidos para AVISOS:

- Prova
- Trabalho
- Evento
- Aviso
- HorarioExtra

Regra importante: a grade fixa fica em `HORARIO_SEMANAL`. Alteracoes pontuais, reposicoes, aula extra ou mudanca fora da rotina entram em `AVISOS` como `HorarioExtra`.

## Materias envolvidas

1. Programacao Aplicada a Inteligencia Artificial I
2. Tecnologias Emergentes em Inteligencia Artificial
3. Fundamentos de Inteligencia Artificial
4. Desenvolvimento Local

## Funcao de cada materia no projeto

### Programacao Aplicada a IA I

Construir o sistema, codar o Web App, trabalhar entrada, processamento, saida, logica, testes e consultas.

### Tecnologias Emergentes em IA

Compreender chatbot, assistente virtual, NLP, intencao, fallback, arquitetura de conversa e tecnologias emergentes ligadas ao projeto.

### Fundamentos de IA

Discutir IA simbolica, automacao, limites do sistema, etica, checagem, riscos e regra de nao inventar informacao.

### Desenvolvimento Local

Investigar o problema real da comunicacao escolar, justificar a solucao, cuidar da LGPD, registrar diario de bordo, definir criterios de implantacao e impacto.

## Estado atual

O projeto esta no comeco pratico. Existe a planilha com os dados, mas o sistema ainda esta sendo construido do zero.

MVP 0 ja iniciado:

- `index.html`: tela inicial do chat.
- `Main.gs`: `doGet()` para abrir o HTML e `responderPergunta()` com resposta de teste/mock.

## Proximas microentregas planejadas para o index.html

1. Indicador "Processando..." enquanto o bot responde.
2. Botao "Limpar conversa".
3. Botoes de perguntas prontas.
4. Historico no navegador com `localStorage`.
5. Hora HH:mm em cada mensagem.
6. Painel "O que posso perguntar?" com exemplos clicaveis.

## Regra pedagogica para codigo

Todo codigo deve ser muito comentado, didatico e explicado passo a passo, pois os alunos sao iniciantes.

Quando a alteracao for pequena, nao reescrever o arquivo inteiro. Mostrar:

1. O que sera mudado.
2. Bloco antigo.
3. Bloco novo.
4. Explicacao das diferencas.
5. Checklist de teste.

Prompt padrao dos alunos:

> Vou colar o index.html COMPLETO. Faça a alteração pedida SEM reescrever o arquivo inteiro. Mostre BLOCO ANTIGO e BLOCO NOVO para substituição. Explique as diferenças e entregue checklist de testes. Alterar apenas index.html, sem mexer no Main.gs.

## Abordagem pedagogica

- Turma iniciante.
- Trabalho leve, progressivo e pratico.
- Cada aula deve gerar uma pequena entrega visivel.
- Prioridade atual: sair da teoria e construir um sistema conceitual funcional para que os alunos vejam progresso real.

## Regra permanente

Nao inventar conteudos fora dos objetos de conhecimento oficiais das materias. Sempre alinhar ao projeto Central de Avisos e ao nivel iniciante da turma.
