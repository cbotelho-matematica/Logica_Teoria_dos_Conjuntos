1. (ENDERTON, p. 6) Quais das sentenças abaixo tornam-se verdadeiras quando inserimos "$\displaystyle \in$" nas lacunas? Quais se tornam verdadeiras, se inserimos "$\displaystyle \subseteq$"?

**a.)** $\displaystyle \{ \emptyset \} \_\_\_\_ \{ \emptyset, \{ \emptyset \}\}$

<details>
<summary><strong>Resposta</strong></summary>

Observe que qualquer um dos dois sinais torna a sentença verdadeira. Vejamos a justificativa:

- Por definição, dizemos $A \subseteq B \iff \forall x \in A \rightarrow x \in B$. Como o conjunto da direitra possui somente o elemento $\emptyset$ e este também é elemento do conjunto da esquerda, a relação de **inclusão** está verificada.
- Por definição, $x \in B$ se $x$ é um elemento de $B$. O conjunto da direita possui dois elementos: $\emptyset$ e $\left\{ \emptyset \right\}$. O conjunto da esquerda $\left(\left\{ \emptyset \right\}\right)$  é, portanto, elemento do conjunto da direita e a relação de **pertinência** é observada.
</details>

<br />

**b.)** $\displaystyle \left\{ \empty \right\} \_\_\_\_ \left\{ \empty, \left\{\left\{ \empty \right\}\right\}\right\}$

<details>
<summary><strong>Resposta</strong></summary>

Observa-se que $\forall \; x \in A \rightarrow x \in B$. Logo, por definição, a relação de **inclusão** $(\subseteq)$ é verdadeira.

</details>

<br />

c. $\left\{ \left\{ \empty \right\} \right\} \_\_\_\_ \left\{  \empty,  \left\{ \empty  \right\}   \right\}$

<details>
<summary><strong>Resposta</strong></summary>

O conjunto da esquerda possui somente um elemento: $\left\{ \emptyset \right\}$. Verifica-se que este também é elemento do conjunto da direita. Logo, como cada elemento de A está em B, observa-se a relação de inclusão $(\subseteqq)$
</details>
<br />

d. $\left\{ \left\{ \empty \right\} \right\} \_\_\_\_ \left\{  \empty,  \left\{\left\{ \empty  \right\}\right\}   \right\}$

<details>
<summary><strong>Resposta</strong></summary>

Como o conjunto da esquerda é elemento do conjunto da direita, observa-se a relação de pertinência $(\in)$.
</details>

<br />

e. $\left\{\left\{ \empty \right\}\right\} \_\_\_\_ \left\{ \empty, \left\{  \empty , \left\{ \empty \right\} \right\} \right\}$ 

<details>
<summary><strong>Resposta</strong></summary>

**Nenhuma das duas relações é observada**. Chamemos $A$ ao conjunto da esquerda e $B$ ao conjunto da direita:

- $A = \{\{\emptyset\}\}$
- $B= \{\emptyset, \{ \emptyset, \{\emptyset\} \}\}$

Observe que o único elemento de $A$ não pertence a $B$, $\{\emptyset\} \not\in B$. Logo $A \not\subseteq B$.

  Observe também que os elementos de $B$ são dois:
  - $\emptyset$;
  - $\{\emptyset, \{ \emptyset \}\}$

  Como ambos são diferentes de $A = \{\{\emptyset\}\}$, então $A \not\in B$.
</details>

<br />
<hr />
<br />

2. (ENDERTON, p. 7) Demonstre que nenhum desses três conjuntos: $\empty, \left\{ \empty \right\}, \left\{ \left\{ \empty \right\} \right\}$ é igual ao outro.

<details>
<summary><strong>Resposta</strong></summary>

A relação de igualdade entre conjuntos é definida da seguinte forma: Dados dois conjuntos $A, B$, $A=B$ se, e somente se, $\forall \, x \in A \rightarrow x \in B$ e se $\forall \, x \in B \rightarrow x \in A$. Ou seja, dois conjuntos serão iguais se: $A \subseteq B$ e $B \subseteq A$.
Para respondermos ao problema, chamemos os conjuntos de:

- $A = \emptyset$
- $B = \{ \emptyset \}$
- $C = \{\{ \emptyset \}\}$

Observe que $A \subseteq B$, pois o conjunto vazio é subconjunto de qualquer outro, por vacuidade, mas $B \not\subseteq A$, pois $A$ não possui elementos. Da mesma forma $A \subseteq C$, mas $C \not\subseteq A$. Portanto $A \neq B$ e $A \neq C$.

Resta somente compararmos $B$ e $C$. Notemos que $B \not\subseteq C$. Compare os elementos de cada conjunto e verique que $\emptyset \neq \{ \emptyset \}$. Portando descarta-se a igualdade entre ambos: $B \neq C$. $\blacksquare$
</details>

<br />
<hr />
<br />

3. (ENDERTON, p. 7) Demonstre que:

$$
B \subseteq C \rightarrow \mathcal{P}(B) \subseteq \mathcal{P}(C)
$$

<details>
<summary><strong>Resposta</strong></summary>

Se $B \subseteq C$, então, por definição $\forall \; x \in B \rightarrow x \in C$. Ou seja, cada elemento de $B$ é também elemento de $C$.

Observemos que $\mathcal{P}(B)$ é o conjunto formado por todos os subconjuntos de $B$. Cada um dos subconjuntos ou é o conjunto vazio ou é o conjunto formado por um ou mais elementos de $B$.

De modo semelhante, $\mathcal{P}(C)$ é o conjunto formado por todos os subconjuntos de $C$. Note que o conjunto vazio também é subconjunto de $\mathcal{P}(C)$ e também serão subcojuntos os conjuntos formados por um ou mais elementos de $C$.

Como vimos, cada elemento de $B$ é elemento de $C$, então, pela definição do conjunto das partes, cada subconjunto de $B$ será subconjunto de $C$. Portanto, considerando um subconjunto $X$ qualquer de $B$:

$$
\forall \; X \in \mathcal{P}(B) \rightarrow X \in  \mathcal{P}(C) \implies \mathcal{P}(B) \subseteq  \mathcal{P}(C)
$$
</details>

<br />
<hr />
<br />

4. (ENDERTON, p. 7) Considerando $x$ e $y$ elementos de $B$. Prove que $\left\{ \left\{ x \right\}, \left\{ x,y \right\} \right\} \in \mathcal{P}\mathcal{P}(B).$

<details>
<summary>Resposta</summary>

Se $x,y \in B$, então:

$$
\{ x \} \subset B \land \{ x,y \} \subset B
$$

Logo:

$$
\{x\} \in \mathcal{P}(B) \land \{x,y\} \in \mathcal{P(B)}
$$

Sendo assim, pela definição do conjunto das partes:

$$
\{ \{x\}, \{x,y\} \} \subset \mathcal{P(B)}
$$
</details>
