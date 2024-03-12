Choses à connaître pour le contrôle : 

1. Faire un arbre de probabilité :

	![[Pasted image 20240312045439.png]]

2. Connaître les formules de probabilités conditionnelles : 

	$$
	\begin{align*} 
	P_B(A) &= \frac{P(A \cup B)}{P(B)} \\ P_A(B) &= \frac{P(A \cup B)}{P(A)}
	\end{align*}
	$$
	Et par réciproque : 
	$$
	P(A \cup B) = P_B(A) \times P(B) = P_A(B) \times P(A)
	$$
	
	**L'ensemble des chemins qui aboutissent à l'évènement A, forme la probabilité $P(A)$.**

	On **additionne les chemins** mais on **multiplie** les sous-chemins d'un même chemin.

3. Qu'est ce qu'une épreuve de Bernoulli

	On appelle épreuve de Bernoulli de paramètre p, une expérience aléatoire ayant deux issues : l'une nommée "Succès" notée $S$, de probabilité $p$, et l'autre "échec" notée $\bar{S}$ de probabilité $1-p$

5. Différence entre épreuve de Bernoulli et schéma de Bernoulli 

	Un schéma de Bernoulli est une répétition de n fois, une même épreuve de bernoulli. Répété de manière identique et indépendante.

4. Définir une loi binomiale :

	Prenons par exemple, un pile ou face, sur 10 parties. ($A$ : Pile, $\bar{A}$ : Face)

	On répète 10 fois de manière **identique et indépendante** la même épreuve de Bernoulli à deux issues (dont le succès est « Obtenir pile ») de paramètre p = 0.5.
	
	Donc on a un schéma de Bernoulli de paramètres n = 10 et p = 0.5. La variable aléatoire X qui compte le nombre de succès suit la loi binomiale $\beta$(10 ; 0.5).

5. Appliquer une loi binomiale : 

	Formule de probabilité : 
	$$
	\begin{align*}
	P(X = k) &= \binom{n}{k} \times p^k \times (1-p)^{n-k} \\
	P(X = 0) &= (1-p)^{n}\\
	P(X = n) &= p^{n}\\
	P(X = 1) &= n \times p \times (1-p)^{n-1}\\
	P(X = n-1) &= n \times p^{n-1} \times (1-p)
	\end{align*}
	$$

	Grâce à la définition d'une épreuve de Bernouli, on peut établir les relations : 
	$$
	\begin{align*}
	P(X \geq 1) &= 1-P(X = 0) \\
	P(X>3) &= 1-P(X \leq3)\\
	P(X <3) &= P(X \leq 2) \\
	P(X \geq3) &= 1- P(X \leq 2) \\
	P(1 \leq X\leq3) &= P(X \leq 3) - P(X=0) \\
	P(1 < X <3) &= P(X =2)
	\end{align*}
	$$
6. Trouver un nombre n de parties.
	Si on cherche par exemple, le nombre n de parties, pour que la probablité que au moins 1 succès se produise sois supérieur à 90% :

	On traduis l'énoncé : $P(X \geq 1) > 0.90$  

	On résous :

	$$
	\begin{align*}
	P(X \geq 1) &> 0.90 \\
	1 - P(X =0 ) &> 0.90 \\
	-P(X=0)&> -0.10 \\
	P(X=0)&< 0.10 \\
	(1-p)^n &< 0.10 \\
	n\times\ln(1-p) &< \ln(0.10)\\
	n &> \frac{\ln(0.10)}{\ln(1-p)}
	\end{align*}
	$$
	Remarque : On n'oublie pas de justifier que le sens des inégalités changent, car $\ln(x<1)<0$
	
1. Calculer une espérance : 

	$E(X) = n \times p$, L'Espérance est le nombre de moyen, auquel ce succès devrait occurée à la fin des n parties. 

	Ex : On appelle des personnes au téléphone, et on regarde si elles décrochent ou non.
	
	X suit $\beta(3000, 0.4)$, $E(X) = 3000 \times 0.4 = 1200$. Sur les 3000 personnes, on peut espérer que en moyenne 1200 personnes répondent. 

	Remarque : Il est également possible de trouver n, si l'espérance, et p sont donné.
	![[Pasted image 20240312045252.png]]