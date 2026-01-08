# O que é Inferência Causal?

De forma simples vamos analisar os componentes dessa expressão:

- **Inferência**: O ato de tirar conclusões baseadas em evidências a partir de dados.
- **Causal**: A relação entre causa e efeito, onde uma variável (a causa) influencia ou determina outra variável (o efeito).

Aqui iremos aprender como identificar e medir o impacto de intervenções ou mudanças, indo além da simples observação de correlações entre variáveis. Quando digo intervenções, estou me referindo a ações deliberadas que podem ser tomadas para alterar o estado de um sistema[^1], como implementar uma nova política, lançar um novo produto ou modificar um processo existente.

Mais comumente desejamos saber qual impacto de uma certa ação em um resultado de interesse. Por exemplo, uma empresa pode querer saber qual o impacto de uma **campanha de marketing** nas vendas de um produto, ou um governo pode querer entender o efeito de uma nova política pública na saúde da população.

## É por causa ou por acaso?

Nós humanos somos muito bons em encontrar padrões e descobrir correlações entre eventos. No entanto, é crucial entender que correlação não implica causalidade. Apenas porque dois eventos ocorrem juntos, não significa que um causa o outro.

Um exemplo intuitivo é a correlação entre o aumento de preços das diárias de hotéis e o aumento do número de turistas em uma cidade. Embora esses dois eventos estejam correlacionados, não podemos concluir que o aumento dos preços das diárias de hotéis causa o aumento do número de turistas. Na verdade, é mais provável que ambos os eventos sejam causados por um terceiro fator, como a alta temporada turística.

![Correlação Espúria](../assets/imgs/spurious_correlation_example.svg){ align=right width=500px }

Você pode encontrar no site [Spurious Correlations](https://www.tylervigen.com/) diversos exemplos engraçados de correlações espúrias[^2], como por exemploa correlação entre o consumo de margarina e o número de divórcios em Maine. Embora esses dois eventos possam estar correlacionados, não há uma relação causal direta entre eles, pois mesmo se o estado do Maine pare de consumir margarina, isso não afetará o número de divórcios.

Esses exemplos destacam a importância de não tirar conclusões precipitadas com base apenas em correlações observadas. Para estabelecer uma relação causal, é necessário realizar análises mais aprofundadas, que iremos aprender ao longo deste livro.

Se você não está familiarizado com o conceito de correlação, vamos revisitar este conceito rapidamente antes de avançarmos para a causalidade. Clique aqui para revisar conceito de [correlação](./Estatística/Correlação/Teoria.md) e explorar o conceito com exemplos práticos.

## Causalidade

O grande desafio da inferência causal é determinar se uma variável causa mudanças em outra variável. A causalidade implica que uma mudança em uma variável (a causa) leva a uma mudança em outra variável (o efeito). Estabelecer causalidade é mais complexo do que simplesmente observar correlações, pois requer a consideração de outros fatores, como variáveis de confusão, viés de seleção e a direção da relação causal que veremos mais adiante.

Para nos ajudar a determinar relações causais preciremos enteder o modelo de resultados potenciais, que será nossa base para o estudo de inferência causal ao longo deste livro.

### Resultados Potenciais



As correlações são muito úteis para fazer previsões e são amplamente utilizadas em modelos preditivos. No entanto, quando se trata de entender o impacto de intervenções ou mudanças em um sistema, a inferência causal é essencial. Por exemplo, se uma empresa deseja saber se aumentar o orçamento de marketing resultará em um aumento nas vendas, a correlação entre o orçamento de marketing e as vendas pode fornecer algumas informações, mas não é suficiente para estabelecer uma relação causal. A empresa precisa entender se o aumento do orçamento de marketing realmente causa um aumento nas vendas, ou se outros fatores estão influenciando essa relação.


[^1]: Um sistema pode ser qualquer conjunto de elementos interconectados que funcionam juntos para atingir um objetivo comum. Pode ser um sistema econômico, social, biológico, tecnológico, entre outros.
[^2]: Correlação Espúria é uma relação entre duas variáveis que parecem estar relacionadas, mas na verdade não há uma conexão causal entre elas. Essas correlações podem ocorrer por acaso ou devido à influência de uma terceira variável não considerada.