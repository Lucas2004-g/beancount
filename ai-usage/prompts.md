# Registro de Uso de Inteligência Artificial

## Contexto de Utilização
A Inteligência Artificial foi utilizada como copiloto arquitetural e de engenharia de requisitos para mapear o comportamento do ecossistema do Beancount (ferramenta open-source de contabilidade em texto puro) e estruturar a documentation de engenharia de software de um assistente auxiliar.

## Prompts Utilizados

### 1. Descoberta e Contexto (Discovery)
> "Atue como um Engenheiro de Software sênior especialista em finanças e contabilidade de dupla entrada. Preciso estruturar a fase de Discovery para um assistente que ajuda usuários do Beancount a não errarem a sintaxe de seus arquivos. Crie o JTBD e duas personas detalhadas (uma técnica e uma não-técnica) focadas nas dores de escrita manual."

### 2. Engenharia de Requisitos e Backlog
> "Com base nas personas criadas para o assistente Beancount, monte um backlog com 5 Histórias de Usuário completas seguindo o padrão 'Como... Quero... Para que...'. Adicione também 3 cenários de teste práticos detalhando o comportamento esperado de sucesso e falha de balanceamento de moedas."

### 3. Implementação do Script Validador
> "Gere um script em Python simples e robusto chamado `bean_wizard.py` que simule esse assistente. Ele deve receber uma string de transação, validar via Regex se a data está no formato YYYY-MM-DD e checar aritmeticamente se os valores de débito e crédito passados se anulam (somam zero)."