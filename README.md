# **Análise [gqs-algoritmo-01-py] - Palíndromos**

### **Nível 1: O Básico da Investigação**

##### **O que o código faz:** 

Pega uma variável remove números e espaço, reduz um texto para letra minúscula e vê se a frase lendo de trás pra frente é igual lendo normalmente.

##### **Como executar:** 

Ajuste a frase na variável texto1 ou texto2 e use o https://www.online-python.com/, copie o código existente em ``` DesafioLogica.py ``` e cole no quadro onde esta o main.py (substituindo todo código já existente no site) e clique em RUN

##### **Exemplo de saída:** 

Com o padrão do código:

```texto1 = "A sacada da casa de cadasa" ```

```texto2 = "Socorram-me, subi no ônibus em Marrocos" ```

A primeira é apresentada FALSE e a segunda é TRUE:

~~~
Teste 1: False
Teste 2: True
~~~

### **Nível 2: Engenharia Reversa e Análise de Comportamento**

##### **Desvendando os métodos:**

###### **Função do Main:** 

Se o nome do arquivo for main, ele executa toda a rotina do programa.

###### **Análise código:**

* *def analisar(entrada):* faz a execução do programa;

* *if entrada is none:* faz a validação se existe alguma entrada a ser analisada, se não tiver nenhuma entrada, sai do programa \[*return false*];

* *limpa = re.sub(r'\[^a-zA-Z0-9]', '', entrada).lower()*: remove todas os números e coloca tudo em caixa baixa;

* *invertida = limpa\[::-1]:* inverte toda a string, mudando a ordem do caracteres

* *return limpa == invertida:* valida se a string invertida é igual a string original

###### **O Mistério dos Testes:**
* O primeiro texto ```A sacada da casa de cadasa```, juntando tudo o resultado é ```asadacedasacadadacasa``` que não é igual ao texto digitado
* O segundo texto ```Socorram-me, subi no ônibus em Marrocos```, é idêntico quando invertido: ```socorrammesubinonibusemmarrocos```

---

##  Sobre o Autor 

Este projeto é um *fork* original do **Prof Daniel Paiva** (https://github.com/danhpaiva/gqs-algoritmo-01-py) e documentado por **Arthur Marques Diniz**.

*   **GitHub:** [@arthurmdiniz](https://github.com)
*   **LinkedIn:** [arthurmdiniz](https://www.linkedin.com/in/arthurmdiniz/)
*   **E-mail:** arthurmdiniz@outlook.com.br

Sinta-se à vontade para enviar *pull requests*, reportar problemas ou propor melhorias!

  






