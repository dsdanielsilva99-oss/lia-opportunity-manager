# Painel das seis oportunidades — LIA UFSCar

**Daniel Silva Santos** · área de interesse: **Relações Institucionais** · Processo seletivo 2026.2

Aplicação para a Liga de Inteligência Artificial da UFSCar acompanhar as seis oportunidades do case
“Seis portas, uma Liga”. Ela responde três perguntas sem precisar de explicação verbal: **o que vence
primeiro, o que está em espera e quais compromissos já podem ser assumidos** — além de registrar, para
cada organização, a decisão tomada, a justificativa, a próxima ação com responsável e prazo, as
informações pendentes e a dedicação estimada da equipe.

A ideia é simples: se eu sair da Liga amanhã, outra pessoa abre este arquivo e continua o trabalho.

---

## Como abrir e testar

1. Baixe ou clone o repositório.
2. Abra o arquivo **`index.html`** com dois cliques, em qualquer navegador.

Não há instalação, servidor, build, login, banco de dados, API ou serviço pago. Funciona offline e em
um arquivo único.

**Roteiro de teste em dois minutos:**

| Passo | O que você deve ver |
|---|---|
| Abrir a aba **Agenda** | A régua mostra que o primeiro prazo a vencer é o da **Meridian, em 01/10** — e não o da Senda, que é a organização nº 01 do case. |
| Ler as três filas | O que pode ser assumido agora, o que está em espera e o que **não** será assumido, com o motivo de cada renúncia. |
| Marcar um compromisso | A barra avança e o indicador de cumprimento muda sozinho na aba **Indicadores**. A marcação fica salva neste navegador. |
| Aba **Oportunidades** | Filtre por “Prioridade 1” e veja as duas que vencem primeiro. Abra o cartão da Senda para ver decisão, pendências e condições de revisão. |
| Aba **Equipe e capacidade** | A grade semanal mostra que o pico é de **5 dos 6 membros**, entre 20/10 e 31/10. |
| Aba **Primeira mensagem** | O rascunho completo do primeiro contato, pronto para copiar. |
| Aba **Plano e renúncias** | O raciocínio inteiro: critérios, suposições declaradas e o que fica de fora. |

Testado em Chrome, Firefox e Safari, em desktop e celular.

---

## O que está no repositório

```
index.html                       aplicação completa (HTML + CSS + JavaScript, arquivo único)
docs/
  MENSAGEM_02_SENDA.md           rascunho do segundo contato
  diario_de_bordo.pdf            diário de bordo em três páginas
```

---

## O plano, em resumo

Seis convites chegaram a uma Liga de seis pessoas que ainda não entregou nada externamente. O risco não
é escolher a oportunidade errada: é tratar seis convites como seis projetos e não concluir nenhum. Por
isso as oportunidades foram classificadas pelo **tipo de compromisso** que exigem, não pelo porte de
quem convidou.

| Prazo | Organização | Decisão | Dedicação |
|---|---|---|---|
| 01/10 | Meridian Estratégia | Confirmar a oficina de uma manhã | 2 membros · preparação + 1 manhã |
| 02/10 | Senda Patrimonial | Aceitar a conversa e abrir o piloto de 4 semanas | 2 membros · 4 semanas |
| 07/10 | Brava Consultoria | Aceitar a formação com turma de 3 | 3 membros · 6 semanas |
| semana de 05/10 | Violeta Financeira | Conversa de 30 min, sem prometer projeto | 1 a 2 membros · pontual |
| 15/10 | Prisma Estratégica | Conversa de 20 min e candidatura enxuta | 1 membro · ~1 dia somado |
| 16/10 | Aerion Sistemas | Interesse, perguntas e visita em novembro | 1 a 2 membros · pontual |

**Regra de proteção.** A LIA não abre uma segunda frente de execução externa enquanto o piloto Senda
estiver em andamento. Conversas, candidaturas, oficinas e visitas continuam, porque consomem horas
pontuais e não dedicação constante.

**O que fica de fora, de propósito:** projeto de três meses na Violeta, projeto de cinco meses na
Aerion, segundo piloto em paralelo, e reserva de equipe para o desafio da Prisma em novembro. Os motivos
estão na aba **Plano e renúncias**.

**Indicadores:** cumprimento dos compromissos (≥ 90%), relações com próximo passo definido (≥ 50%) e
membros com dedicação estruturada (máx. 5 de 6).

---

## Responsabilidades por função

O cenário não informa quem são os seis integrantes, então nenhum nome foi inventado. As
responsabilidades são distribuídas por função: Relações Institucionais, Coordenação de projeto, Apoio
técnico, Coordenação de formação, Operações, e Registro e síntese. A alocação nominal só deve ser feita
quando os integrantes forem conhecidos.

---

## Notas técnicas

- Arquivo único, sem dependências externas e sem requisições de rede — abre por `file://`.
- Os dados das seis oportunidades ficam em uma lista no início do script; a interface é desenhada a
  partir dela. Mudar uma decisão em um lugar atualiza cartões, régua e filtros ao mesmo tempo.
- As marcações de compromisso usam `localStorage`, protegido por tratamento de erro — em navegador com
  armazenamento bloqueado a página continua funcionando, apenas sem guardar as marcações.
- Responsivo até 390 px, com foco de teclado visível e respeito a `prefers-reduced-motion`.
- A aplicação foi construída com apoio do **Antigravity IDE**, conforme orientado no material. O registro
  do uso de IA está no diário de bordo.

---

## Sobre as datas

As datas entre 01/10/2026 e 16/10/2026 são os **prazos apresentados no cenário do case**. Nada aqui
afirma que contatos, reuniões ou atividades já tenham ocorrido. Todas as organizações, pessoas e
conversas são fictícias, conforme o material.

---

## Referências

OLIVEIRA, Tiago Chaves. *Guia referencial para gerenciamento de projetos e portfólios de projetos*.
Brasília, DF: Escola Nacional de Administração Pública, 2021. Disponível em:
https://repositorio.enap.gov.br/handle/1/6155. Acesso em: 6 out. 2026.

LIGA IA UFSCAR. *Seis portas, uma Liga: case para novos founders — Processo seletivo 2026.2*. [S. l.],
2026.
