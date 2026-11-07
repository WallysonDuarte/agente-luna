---
name: email-marketing
description: Construir sequencias, garantir entregabilidade e medir com honestidade o canal de maior retorno.
---

# E-mail marketing

## Quando usar

Boas-vindas, nutricao, reativacao, recuperacao de carrinho, comunicado.

## Entregabilidade primeiro

Lista boa com reputacao ruim nao entrega. Antes de qualquer envio:

- Registros de autenticacao de dominio configurados: autorizacao de remetente, assinatura
  criptografica e politica de alinhamento.
- Politica de alinhamento em modo de rejeicao assim que a assinatura estiver estavel. Encaminhamento
  sem validacao propaga falsificacao mesmo com a politica correta publicada — a validacao precisa
  acontecer no recebimento.
- Aquecimento de dominio novo: volume crescente ao longo de semanas.
- Limpeza de lista: remova endereco invalido e quem nao abre por longo periodo.
- Link de descadastro visivel e funcionando com um clique.

Aceitacao pelo provedor de envio **nao** garante entrega: teste com caixa real do principal
provedor de e-mail do seu publico antes de confiar.

## Sequencias

### Boas-vindas
1. Entrega do que foi prometido, imediata.
2. Quem somos e por que confiar (prova, caso real).
3. Valor gratuito aplicavel sem comprar nada.
4. Oferta, com objecao principal respondida.

### Nutricao
A cada dois ou tres dias, um objetivo por mensagem, sempre com algo util antes do pedido.

### Reativacao
Para quem nao abre ha semanas: assunto direto perguntando se deve continuar enviando, com opcao de
reduzir frequencia em vez de descadastrar.

### Recuperacao de carrinho
Primeira mensagem em uma hora (lembrete), segunda em 24 horas (objecao), terceira em 72 horas
(incentivo, se houver). Nunca mais que tres.

## Escrita

- **Assunto:** abaixo de 50 caracteres, uma ideia, curiosidade ou beneficio concreto. Sem letras
  maiusculas em excesso e sem pontuacao repetida.
- **Texto de previa:** complementa o assunto, nao repete. Ate 90 caracteres.
- **Corpo:** um objetivo, escaneavel, chamada unica e clara.
- **Remetente:** nome de pessoa costuma superar nome de empresa.
- **Horario:** teste; nao copie regra generica.

## Segmentacao

Por estagio no funil e por engajamento. Enviar a mesma mensagem para toda a lista queima
reputacao: quem nao tem interesse marca como indesejado e derruba a entrega de quem tem.

## Metricas

| Metrica | Referencia | Cuidado |
|---|---|---|
| Entrega | acima de 98% | abaixo disso, problema tecnico |
| Abertura | acima de 20% | inflada por carregamento automatico de imagem |
| Clique | acima de 2,5% | metrica mais confiavel que abertura |
| Descadastro | abaixo de 0,5% | acima, frequencia ou segmentacao erradas |
| Marcacao como indesejado | abaixo de 0,1% | acima, risco de bloqueio do dominio |

## Envio automatico: janela e contexto

Rotina que envia mensagem automatica precisa de janela de horario respeitada em **duas camadas**:
o processo adia o ciclo fora da janela (itens ficam pendentes, sem registrar falha) e o servico de
envio recusa como ultima defesa. Fluxos disparados pelo usuario (segundo fator, recuperacao de
senha) **nao** entram na janela.

Converta o horario do servidor para o fuso do publico e teste as quatro bordas da janela.

## Checklist

- [ ] Autenticacao de dominio configurada e validada
- [ ] Teste de entrega em caixa real do principal provedor
- [ ] Lista limpa; descadastro em um clique
- [ ] Sequencia com um objetivo por mensagem
- [ ] Segmentacao por estagio e engajamento
- [ ] Janela de horario respeitada no automatico, nao no transacional
- [ ] Metricas acompanhadas, decisao pelo clique

## Pronto quando

A taxa de entrega esta acima de 98%, a marcacao como indesejado abaixo de 0,1%, e cada sequencia
tem um objetivo por mensagem.
