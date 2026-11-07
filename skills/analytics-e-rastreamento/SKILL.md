---
name: analytics-e-rastreamento
description: Instrumentar eventos, parametros de origem e funis para atribuir resultado com honestidade.
---

# Analytics e rastreamento

## Quando usar

Antes de qualquer trafego pago, ao criar fluxo novo, ao duvidar de um numero.

## Parametros de origem

Padronize e **documente**; parametro escrito de duas formas diferentes gera dois relatorios:

```
?origem=<canal>&meio=<tipo>&campanha=<nome>&conteudo=<variacao>&termo=<palavra>
```

Regras: tudo em minusculas, sem acento, separador unico (hifen), nome de campanha com data
(`lancamento-2026-11`). Mantenha uma planilha de referencia — ela e a diferenca entre relatorio
legivel e sopa de letras.

## Eventos

Instrumente o **funil**, nao cada clique:

| Evento | Quando dispara |
|---|---|
| visualizou_oferta | pagina de preco carregou |
| iniciou_cadastro | primeiro campo preenchido |
| concluiu_cadastro | conta criada |
| ativou | primeiro valor entregue |
| iniciou_pagamento | checkout aberto |
| converteu | pagamento confirmado **no servidor** |

Conversao que importa se confirma no servidor, nao no navegador: bloqueador de script e aba fechada
derrubam o evento do cliente.

Nomeie com verbo no passado e padrao unico. Nunca envie dado pessoal nem identificador sensivel em
parametro de URL ou propriedade de evento.

## Teste do rastreamento

Antes de gastar em trafego:

1. Percorra o funil completo e confira que **cada** evento chegou.
2. Confira os parametros de origem no relatorio em tempo real.
3. Faca uma conversao de teste e confirme o valor e a moeda.
4. Verifique que recarregar a pagina nao duplica o evento.

Rastreamento nao testado e a causa mais comum de "a campanha nao trouxe nada".

## Atribuicao: seja honesto

- Ultimo clique superestima o canal de fechamento (busca de marca, remarketing).
- Primeiro clique superestima descoberta.
- Quando duas acoes aconteceram na mesma semana, **nao da para atribuir** com confianca. Diga isso
  em vez de escolher o numero conveniente.
- Compare periodos equivalentes: semana com feriado nao se compara com semana cheia.

## Armadilhas de leitura

- **Metrica de vanidade:** total acumulado sempre sobe. Use taxa e periodo.
- **Media escondendo cauda:** olhe percentis.
- **Denominador movel:** mudar a definicao de "ativo" no meio invalida a serie.
- **Fuso horario:** agregado em tempo universal exibido em data local desloca o dia.
- **Amostragem:** relatorio amostrado em periodo longo distorce segmento pequeno.

## Relatorio

Tres perguntas, sempre: o que mudou, por que mudou, o que fazer. Numero sem leitura e planilha, nao
relatorio. Inclua o que **nao** funcionou — e o que evita repetir o gasto.

## Checklist

- [ ] Parametros padronizados e documentados
- [ ] Eventos do funil instrumentados, com nomes padronizados
- [ ] Conversao confirmada no servidor
- [ ] Funil completo percorrido e cada evento verificado
- [ ] Nenhum dado pessoal em parametro ou propriedade
- [ ] Definicoes de metrica estaveis e escritas
- [ ] Relatorio com leitura e acao

## Pronto quando

O funil completo foi percorrido com todos os eventos verificados, e o relatorio diz o que fazer com
o resultado.
