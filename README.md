# Decodificador e Inversor de Matriz - Cidade Dorme

Bem-vindo ao Decodificador e Inversor de Matriz, uma ferramenta interativa projetada para auxiliar em jogos de mistério e dedução como o "Cidade Dorme"! Esta aplicação web permite calcular a inversa de uma matriz chave e decodificar mensagens que foram criptografadas usando um método similar à Cifra de Hill, adaptado para lidar com números decimais e com uma conversão de alfabeto onde A=1.

## Funcionalidades Principais

A aplicação é dividida em duas ferramentas principais:

### 1. Inversor de Matriz Chave (K)
Esta seção ajuda você a encontrar a matriz inversa (K<sup>-1</sup>) de uma dada Matriz Chave (K).
* **Entrada:** Permite inserir uma Matriz Chave (K) de tamanho 2x2 ou 3x3, com elementos podendo ser números inteiros ou decimais.
* **Cálculo da Inversa:**
    * Calcula o determinante da Matriz Chave K (det(K)).
    * Calcula a Matriz Adjunta de K (adj(K)).
    * Calcula a Matriz Inversa K<sup>-1</sup> usando a fórmula: $K^{-1} = \frac{1}{\text{det}(K)} \times \text{adj}(K)$. Os elementos da K<sup>-1</sup> resultante podem ser números decimais.
* **Passo a Passo:** Exibe as etapas do cálculo (determinante, adjunta e a K<sup>-1</sup> final), com os valores formatados para uma casa decimal.
* **Validação:** Verifica se o determinante é zero; se for, a matriz não é invertível e um erro é indicado.
* **Guia para o Usuário:** Após o cálculo, instrui o usuário a copiar os valores da K<sup>-1</sup> para utilizá-los no decodificador.

### 2. Decodificador de Mensagem
Esta seção decodifica uma mensagem (Matriz Codificada C) usando uma Matriz Chave Invertida (K<sup>-1</sup>).
* **Entrada:**
    * **Matriz Codificada (C):** Permite inserir a matriz que contém a mensagem codificada. Aceita números inteiros ou decimais.
    * **Matriz Chave Invertida (K<sup>-1</sup>):** Permite inserir a matriz inversa da chave (pode ser obtida pelo inversor acima ou inserida manualmente). Aceita números inteiros ou decimais.
    * Seleção do tamanho das matrizes (2x2 ou 3x3).
* **Processo de Decodificação:**
    * Calcula o produto $P_{valores} = C \times K^{-1}$. Os elementos de $P_{valores}$ podem ser decimais.
    * Cada elemento resultante da soma dos produtos é **arredondado** para o número inteiro mais próximo.
    * Este inteiro arredondado é considerado a posição da letra no alfabeto (onde A=1, B=2, ..., Z=26, \_=27).
    * O processo é exibido passo a passo, com destaques visuais para as linhas e colunas sendo multiplicadas, animações dos números e a conversão final para letras.
* **Resultado:**
    * Exibe a "Matriz Decodificada (P) - Valores", mostrando os resultados numéricos (decimais, formatados para uma casa) da multiplicação $C \times K^{-1}$ antes do arredondamento para letras.
    * Exibe a "Mensagem/Identidade Revelada" em letras.
* **Interface Interativa:**
    * Display do alfabeto de referência (A=1, B=2, etc.).
    * Navegação facilitada nos campos da matriz usando a tecla "Enter".

### Outras Funcionalidades
* **Botão "Recomeçar Tudo":** Permite atualizar a página e limpar todos os campos e processos.
* **Design Temático:** Interface com um tema escuro e fontes que remetem ao mistério do jogo "Cidade Dorme".

## Como Usar

1.  **(Opcional) Calcular a K<sup>-1</sup> com o Inversor:**
    * Na seção "Inversor de Matriz Chave (K)", selecione o tamanho da sua Matriz Chave.
    * Preencha os campos com os números da sua Matriz Chave (K).
    * Clique em "Calcular Inversa (K<sup>-1</sup>)".
    * Observe os passos do cálculo e a Matriz Chave Invertida (K<sup>-1</sup>) resultante exibida. Anote ou copie esses valores.

2.  **Decodificar a Mensagem:**
    * Na seção "Decodificador de Mensagem", selecione o tamanho correto das matrizes.
    * Preencha os campos da "Matriz Codificada (C)" com os números da sua mensagem cifrada.
    * Preencha os campos da "Matriz Chave Invertida (K<sup>-1</sup>)" com os valores obtidos pelo inversor (ou com uma K<sup>-1</sup> que você já possua).
    * Clique em "Decodificar Mensagem".

3.  **Observar o Resultado:**
    * Acompanhe o processo de decodificação passo a passo.
    * Veja a "Matriz Decodificada (P) - Valores" e a "Mensagem/Identidade Revelada" final.

4.  **Recomeçar:**
    * Clique no botão "Recomeçar Tudo (Atualizar)" no topo (ou final) da página para limpar tudo e começar de novo.

## Tecnologias Utilizadas

* **HTML5:** Estrutura da página.
* **CSS3:** Estilização, incluindo o uso do framework **Tailwind CSS** para agilidade e estilos personalizados para o tema.
* **JavaScript (ES6+):** Lógica da aplicação, cálculos matemáticos, manipulação do DOM e interatividade.

## Link para Acessar

[Adicione o link para o seu site aqui, por exemplo, o link do GitHub Pages, Netlify ou Vercel, se estiver hospedado]

---

Feito com ❤️ para os mestres e jogadores de Cidade Dorme!
