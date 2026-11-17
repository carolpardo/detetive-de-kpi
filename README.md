# detetive-de-kpi 🕵️

Skill para o Claude que ajuda gestores de indústria a montar a estratégia de um KPI: entender o processo, analisar os dados, achar a causa raiz e sair com um plano de ação.

A skill não entrega uma resposta pronta. Ela conduz a conversa como um consultor de Excelência Operacional, numa ordem fixa:

1. **Entender o processo**: indústria, área, gargalo e turnos. Opcionalmente lê um P&ID, uma tela do supervisório ou um manual.
2. **Entender o KPI**: fórmula, polaridade e, antes de tudo, como o dado é medido.
3. **Definir a meta**: baseline do trimestre anterior, meta, rampa mês a mês e checagem SMART.
4. **Analisar os dados**: lê o seu arquivo (CSV/Excel) em Python e faz Paretos camada por camada (turno → equipamento → tipo de problema → descrição), destacando o que precisa ser tratado para fechar o gap.
5. **Achar a causa raiz**: espinha de peixe (6M) e 5 porquês, com perguntas a quem conhece a linha, mais boas práticas pesquisadas em fontes confiáveis.
6. **Montar o roadmap**: ações por impacto × dificuldade e plano 5W2H.
7. **Fechar o ciclo**: o que padronizar, treinar e levar para o plano de manutenção, mais a rotina de acompanhamento.

No final, gera um **dashboard** com o resultado de cada etapa e o plano de ação. Deck, one-pager A3 e planilha são opcionais.

O horizonte padrão é **trimestral**: olha os últimos 3 meses e planeja os próximos 3.

## Como instalar

1. Baixe `detetive-de-kpi.zip` (na seção Releases ou no botão **Code → Download ZIP** e compacte a pasta `detetive-de-kpi`).
2. No Claude, vá em **Customize → Skills**, clique em **+**, depois em **Create skill → Upload a skill**.
3. Envie o ZIP. A pasta `detetive-de-kpi` precisa estar na raiz do ZIP.

Precisa da execução de código ativada no Claude, para a análise dos dados.

## Como usar

Peça algo como:

> Quero montar a estratégia para melhorar o OEE da minha linha.

Se tiver, tenha à mão um arquivo com os dados do último trimestre (paradas com turno, equipamento, motivo, descrição e duração).

## Autora

Criada por **Carolina Pardo Oliveira**, engenheira química com 8 anos de experiência em operações industriais, performance e Indústria 4.0.

Quer trocar uma ideia, dar feedback ou contar como usou a skill? Fala comigo:

- LinkedIn: [linkedin.com/in/carolina-pardo-oliveira](https://www.linkedin.com/in/carolina-pardo-oliveira/)
- E-mail: carolinapardooliveira@gmail.com

## Licença

MIT. Veja [LICENSE](LICENSE).
