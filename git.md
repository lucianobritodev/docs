## Escrevendo Commits Messages Com Mais Precisão

A mensagem de commit é algo importante dentro de cada projeto, porém ainda negligenciado por maior parte dos devs. As vezes por priorizar a agilidade na entrega, escrevem mensagens mais curtas, mas que não expressam o peso, escopo e descrição das alteração que estão sendo realizadas. Em outros casos, simplesmente desconhecerem ferramentas disponíveis dentro do git.

Visando preencher esse gap, esse artigo propõe trazer mais informações sobre como escrever commit messages com mais precisão.


## Estrutura Das Mensagens de Commits

Com o objetivo de padronizar a estrutura dos commit messages, eles passarão a seguir a seguinte estrutura: primeiro, definir o tipo de commit, em seguida qual escopo (front ou back) esse commit afetará, logo após, informe a descrição (jornada), seguido do corpo (opcional) e rodapé (opcional).

Os commit messages deve ter a seguinte estruturada:

    [tipo]: [escopo] [descrição]

    [corpo opcional]
    - ...
    - ...
    - ...

    [rodapé opcional(s)]

Para facilitar o entendimento do revisor de código, bem como, melhorar as informações do histórico de commits é importante a utilização dos **`tipos`** de commit que estão sendo realizadas naquele momento. Isso melhora a semântica da mensagem de commit e permite melhor rastreabilidade.

## Tipos de Commit Message Permitidos no Git

`BREAKING CHANGE`: um commit que tem o texto **BREAKING CHANGE** no rodapé do commit ou usa um `!` depois do tipo/escopo, introduz uma grande mudança no código.<br>
`build`: indica mudanças que afetam o processo de build do projeto ou dependências externas.<br>
`chore`: indica mudanças de configuração ou de código que não entram no build de produção.<br>
`ci`: indica alteração em algum arquivo de CI do projeto.<br>
`docs`: indica alteração na documentação do projeto.<br>
`feat`: indica que foi adicionado uma nova funcionalidade no código.<br>
`fix`: indica que houve correção de bug no projeto.<br>
`perf`: indica alterações/melhorias significativas que impactam no desempenho da aplicação.<br>
`refactor`: indica refatoração de determinado bloco de código.<br>
`revert`: indica uma reversão de commit anterior.<br>
`style`: indica que houve alteração apenas no estilo do código, sem mudança de algoritmo.<br>
`test`: indica que houve mudanças na estrutura ou na forma de testar o projeto.<br>

**Exemplo:**

    feat: front - meus investimentos

    - implementado tela de listagem de fundos
    - implementado tela de detalhamento de fundos
    - implementado tela de resumo de fundos
