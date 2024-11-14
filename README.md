# Atualização TypeScript 4.5 para 5.6: Resumo de Mudanças e Novos Recursos

  

Atualização do TypeScript na aplicação NestJS e React, de `"typescript": "^4.5.2"` para `"typescript": "^5.6.3"`.

  

## TypeScript 4.6

  

-  **Erro ao acessar propriedades indefinidas**: Introduziu checagens mais rigorosas, prevenindo acessos a propriedades em `undefined` ou `null`.

![image](https://github.com/user-attachments/assets/6db3c7cd-9c36-4a0b-8b40-ca7456c2fed3)


## TypeScript 4.7

  

-  **Tipos condicionais para JSX**: Agora, a tipagem em JSX lida melhor com tipos complexos, sendo ideal para otimizar interfaces no React. **Exemplo**: O uso de never no caso abaixo força o TypeScript a emitir um erro se borderColor ou backgroundColor for passado com o valor de variant incorreto, ajudando a evitar erros e garantindo que o componente receba somente as props válidas.









![image](https://github.com/user-attachments/assets/22039e13-b2ab-419c-ba2e-4d0b228e21d4)
![image](https://github.com/user-attachments/assets/4c90fd49-ae9c-47c6-aa97-5c99d5fb1f76)



  

## TypeScript 4.8

  

-  **Detecção de `undefined` em templates de string**: Agora, ao interpolar variáveis em templates de string, ele alerta se variáveis podem ser `undefined`.

-  **Suporte a `exactOptionalPropertyTypes`**: Essa opção permite definir propriedades opcionais com mais precisão, útil para melhorar a tipagem em DTOs e interfaces no NestJS.

  

## TypeScript 5.0

  

-  **Modifiers `const` e `type` em parâmetros de tipo**: Adiciona flexibilidade em tipos imutáveis e parametrizações, permitindo `readonly` em inferências de tipos.

-  **Extensões de Decorators**: Melhoria para suporte oficial a decoradores, ótimo para definir decoradores no NestJS.

-  **Suporte a `satisfies`**: Uma palavra-chave nova que garante que um valor cumpre o tipo exato sem forçar a tipagem, o que pode melhorar a legibilidade em validações de tipos.

  

## TypeScript 5.1 a 5.6

  

-  **Parâmetros opcionais em inferência**: Melhor gerenciamento de parâmetros opcionais, facilitando funções mais flexíveis.

-  **Tipagem mais flexível em métodos de array**: Suporte melhorado para métodos como `reduce`, especialmente útil em contextos complexos de array.

-  **`const` em locais de variáveis e inferência de tipos**: Inferência de `const` como tipos literais mais precisa, trazendo mais controle para componentes React.

-  **Suporte a Tipos de Tuplas em `satisfies`**: Agora é possível tipar arrays com tuplas, ajudando a especificar dados com precisão.

  

Essas melhorias podem melhorar a robustez e a clareza do seu código, principalmente em cenários de validação de tipos no NestJS e ao estruturar componentes no React.
