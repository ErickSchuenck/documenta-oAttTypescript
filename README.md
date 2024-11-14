# Atualização TypeScript 4.5 para 5.6: Resumo de Mudanças e Novos Recursos

  

Atualização do TypeScript na aplicação NestJS e React, de `"typescript": "^4.5.2"` para `"typescript": "^5.6.3"`.

  

# TypeScript 4.6

  

 - **Erro ao acessar propriedades indefinidas**: Introduziu checagens mais rigorosas, prevenindo acessos a propriedades em `undefined` ou `null`.

![image](https://github.com/user-attachments/assets/6db3c7cd-9c36-4a0b-8b40-ca7456c2fed3)


# TypeScript 4.7

  

 -  **Tipos condicionais para JSX**: Agora, a tipagem em JSX lida melhor com tipos complexos, sendo ideal para otimizar interfaces no React. **Exemplo**: O uso de never no caso abaixo força o TypeScript a emitir um erro se borderColor ou backgroundColor for passado com o valor de variant incorreto, ajudando a evitar erros e garantindo que o componente receba somente as props válidas.

![image](https://github.com/user-attachments/assets/22039e13-b2ab-419c-ba2e-4d0b228e21d4)
![image](https://github.com/user-attachments/assets/4c90fd49-ae9c-47c6-aa97-5c99d5fb1f76)

# TypeScript 4.8

 -  **Detecção de `undefined` em templates de string**: Agora, ao interpolar variáveis em templates de string, ele alerta se variáveis podem ser `undefined`.

# TypeScript 5.0

 -  **Modifiers `const` e `type` em parâmetros de tipo**: Adiciona flexibilidade em tipos imutáveis e parametrizações, permitindo `readonly` em inferências de tipos.
  
![image](https://github.com/user-attachments/assets/b975a935-966a-422c-83b0-d85ce637ed72)


 - **Suporte a `satisfies`**: Uma palavra-chave nova que garante que um valor cumpre o tipo exato sem forçar a tipagem, o que pode melhorar a legibilidade em validações de tipos. Exemplo de uso do operador:

![image](https://github.com/user-attachments/assets/6dd0c3a6-2242-401b-b70f-89fd5d679539)
![image](https://github.com/user-attachments/assets/3bac10c5-e84e-49e2-9c8c-d2e18782598a)

# TypeScript 5.1 a 5.6

 -  **Parâmetros opcionais em inferência**: Melhor gerenciamento de parâmetros opcionais, facilitando funções mais flexíveis.

![image](https://github.com/user-attachments/assets/057ba27f-ba9d-427e-bea4-8afd31063f8b)
![image](https://github.com/user-attachments/assets/1390943d-9a34-4f73-8cec-b266607a6d4c)

*Com a atualização, o TypeScript infere mais inteligentemente que age é um parâmetro opcional e pode ser tratado diretamente como `number` | `undefined` sem verificações adicionais*



 -  **Tipagem mais flexível em métodos de array**: Suporte melhorado para métodos como `reduce`, especialmente útil em contextos complexos de array.
  *Antes do TypeScript 5.1, ao usar métodos de array como reduce, o TypeScript tinha dificuldades em inferir corretamente o tipo do acumulador (o valor que vai sendo "acumulado" ao longo das iterações). Em muitas situações, você precisaria especificar explicitamente o tipo do acumulador, especialmente quando estava lidando com tipos complexos ou quando o tipo do acumulador dependia do tipo do array.*
   
![image](https://github.com/user-attachments/assets/56fce46f-a72d-4359-a235-691ccde0e074)

 - **`const` em locais de variáveis e inferência de tipos**: Inferência de `const` como tipos literais mais precisa, trazendo mais controle para componentes React.

![image](https://github.com/user-attachments/assets/163aacf6-3424-4572-9ac1-63d9db86eef1)
*Agora, greeting tem o tipo literal "Hello World", e não apenas string. Isso significa que, em vez de permitir qualquer string, o TypeScript agora restringe o valor de greeting ao exato valor "Hello World".*

 - **Suporte a Tipos de Tuplas em `satisfies`**: Agora é possível tipar arrays com tuplas, ajudando a especificar dados com precisão.
*Uma tupla é um tipo de array em que os elementos têm tipos específicos e em posições definidas. Ao contrário de um array tradicional, onde os elementos podem ser de tipos diferentes em qualquer posição, as tuplas têm a vantagem de poderem ser tipadas com diferentes tipos para cada índice.*

![image](https://github.com/user-attachments/assets/2dab6870-eeed-471a-ad3f-90d7ca886785)
