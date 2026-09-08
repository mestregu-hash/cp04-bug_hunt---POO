# Checkpoint 4 — Investigação de Falhas StreamFIAP

## Descrição geral

O **StreamFIAP** é uma API REST destinada ao aluguel de produções audiovisuais
(filmes, séries e documentários), implementada com Spring Boot e Spring Data JPA. O
sistema possibilita o cadastro de conteúdos, sua busca por categoria e a realização
de aluguéis, respeitando regras de negócio como faixa etária indicativa, abatimento
de créditos e valores promocionais.

## Contexto do problema

O código foi disponibilizado com diversos defeitos propositalmente inseridos: falhas
lógicas que não comprometem a compilação (por isso, difíceis de notar em uma
inspeção superficial), falhas no encapsulamento, blocos de tratamento de exceção que
suprimem erros indevidamente, e partes que desrespeitam princípios de Clean Code.

O objetivo é **rastrear, analisar e sanar** esses defeitos — deixando registrado não
apenas a mudança feita, mas também a origem de cada erro e o tópico da disciplina
associado a ele.

## Forma de condução do trabalho

- Inspeção guiada pelos pacotes `model`, `controller` e `exception`, buscando pontos
  onde o comportamento real diverge do esperado.
- Um commit específico para cada ajuste, adotando o padrão de mensagem `fix: bugNN —
  descrição`, garantindo que o histórico do Git narre a apuração de forma
  sequencial.
- Anotação de cada descoberta na tabela a seguir, associando o sintoma percebido à
  linha de código responsável e ao conteúdo correspondente visto em aula.

---

## Identificação

**Grupo:** ___

| Integrante | RM | Turma |
|---|---|---|
| Bento Donato Garcia | 561621 | 2CCPO |
| Enzo Ribeiro Domingues Piazentin | 564216 | 2CCPO |
| Guilherme Domingues Califoni | 565157 | 2CCPO |
| Antonio Lucas Santana Tavares | 565516 | 2CCPO |
| Lucas M. | 563667 | 2CCPO |
| Gustavo Schimith | 564800 | 2CCPO |
