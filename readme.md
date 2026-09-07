# Simulador de Escalonamento de Tarefas

Fork do [enunciado de Sistemas Operacionais](https://github.com/viniciussbrg/simulador-escalonamento). Este repositório contém os documentos e o modelo de entrega; ainda não inclui o simulador, `main.py` ou um executável. As funcionalidades descritas abaixo são requisitos do trabalho, não recursos já implementados neste fork.

O trabalho consiste em desenvolver um simulador de escalonamento de tarefas em
um processador, capaz de reproduzir os algoritmos vistos em sala e o fenômeno
da inversão de prioridades, com seus mecanismos de correção.

O simulador solicitado no enunciado deve implementar seis algoritmos:

- **FCFS** — First-Come, First-Served
- **SJF** — Shortest Job First
- **SRTF** — Shortest Remaining Time First
- **RR** — Round-Robin
- **PRIOc** — Prioridade cooperativa
- **PRIOp** — Prioridade preemptiva

E os mecanismos de tratamento de recursos de uso exclusivo: **inversão de
prioridades**, **herança de prioridade**, **teto de prioridade** e
**envelhecimento**.

## Documentos do projeto

Leia os dois antes de começar.

- [📄 Enunciado](./documentos/01_enunciado.pdf) — o que o simulador precisa
  fazer: os dez requisitos e os cenários de referência
- [📘 Guia de documentação](./documentos/02_guia_documentacao.pdf) — o que
  escrever no README, nos tutoriais e na documentação técnica

O enunciado descreve *o que fazer*; o guia de documentação descreve *como
organizar a entrega*.

## Organização deste repositório

A branch `main` guarda apenas os documentos do projeto e **nunca recebe
entregas**. Cada grupo tem uma **branch dedicada**, onde a entrega aprovada é
incorporada.

### Estado inicial

```
simulador-escalonamento/
└── main
    ├── readme.md
    ├── .gitignore
    └── documentos/
```

### Ao longo do semestre

```
simulador-escalonamento/
├── main       Documentos do projeto (não muda)
├── grupo1     Entrega do grupo 1
├── grupo2     Entrega do grupo 2
├── ...
└── grupo8     Entrega do grupo 8
```

**Como navegar entre as entregas:** clique no seletor de branches, no canto
superior esquerdo, onde aparece `main`, e escolha a branch do grupo desejado.

## Como entregar

A entrega é feita por **fork + pull request**, conforme o guia de entrega
distribuído em aula:

1. **Fazer o fork** deste repositório (botão `Fork`, no canto superior direito)
2. **Clonar o fork** na máquina de um dos integrantes
3. **Desenvolver o trabalho** no fork
4. **Fazer commit e push** a cada avanço, ao longo de todo o desenvolvimento, e
   não apenas no final. O commit registra a alteração no seu computador; só o
   push a envia para o fork, que é o que o GitHub enxerga
5. **Abrir um pull request para a branch do seu grupo**, com o título no
   formato:

```
Entrega - Grupo XX - Nome dos integrantes
```

> **O erro mais comum:** o GitHub oferece `main` como destino por padrão. A
> `main` é protegida e não recebe entregas, então um pull request apontado para
> ela é devolvido sem análise. Troque o campo `base` para a branch do seu grupo
> **antes** de criar o pull request.

## Estrutura esperada dentro do fork

```
simulador-escalonamento/
├── readme.md              como executar, integrantes, funcionalidades
├── Simulador.exe          o arquivo que abre com dois cliques
├── main.py                ponto de entrada do código-fonte
├── simulador/             código-fonte
├── cenarios/              conjuntos de tarefas gravados
└── docs/                  tutoriais e documentação técnica
```

Há um modelo de README de grupo em
[`documentos/modelo_readme_do_grupo.md`](./documentos/modelo_readme_do_grupo.md).
Detalhes do conteúdo no
[guia de documentação](./documentos/02_guia_documentacao.pdf).

## Entregas dos grupos

Entregas aprovadas e incorporadas ao repositório:

<!-- Adicionar conforme os pull requests forem aceitos:
- [Grupo 1](../../tree/grupo1) — Nomes dos integrantes
-->

*Nenhuma entrega aprovada até o momento.*

## Observações

- O projeto precisa **abrir com dois cliques**, sem montagem de ambiente
- Não há relatório escrito: a análise dos resultados é feita oralmente
- Dúvidas: abrir uma **Issue** neste repositório

## Licenciamento

O estado de licenciamento do material de origem está registrado em [license](license). Este fork não acrescenta permissão de reutilização ao código ou aos documentos de terceiros.
