# _**Exercices :**_

### _**Exercice 1 :**_

![[Physique-Chimie/6 Le condensateur et ses applications/Exercice 1.png]]

Dans les schéma `a` et `c`, on a deux conducteurs en regard, séparés par un isolant. Ces deux schémas représentent des condensateurs.
### _**Exercice 2 :**_

![[Physique-Chimie/6 Le condensateur et ses applications/Exercice 2.png]]

1. La charge électrique augmente proportionnellement à la durée d'après le graphique.
2. $I = \frac{\Delta q}{\Delta t} = \frac{6.0 \times 10^{-3}C}{4.0 \times 10^{-3} s} = 1.5A$
### _**Exercice 3 :**_

![[Physique-Chimie/6 Le condensateur et ses applications/Exercice 3.png]]

1. La relation est $q_A = C \times u_C$ avec ici $u_C = u_{AB}$

	La représentation graphique montre que la charge $q$ varie proportionnellement à la tension ; le coefficient de proportionnalité correspond à la capacité du condensateur.

	On a donc $C = \frac{\Delta q_A}{\Delta u_C}$ , Soit ici $C = \frac{6.0\times10^{-6}C}{2.7V}=2.2 \times 10^{-6}F$
2. L'ordre de grandeur de la capacité est le microfarad, qui est un ordre de grandeur usuel 
### _**Exercice 4 :**_

![[Physique-Chimie/6 Le condensateur et ses applications/Exercice 4.png]]

1. A partir de la loi des mailles, montrer que l’équation différentielle régissant l’évolution de $U_c$ s’écrit $U_c + (R+r) \times C \times \frac{dU_c}{dt}=E$
	
	$$
	\begin{align*}U_c+U_r+U_R &= E \end{align*}
	$$
	
	or $\boxed{U_r = r \times i}$ et $\boxed{U_R = R \times i}$
	
	et $\boxed{i = \frac{dq}{dt}=\frac{d(C_{{U}_c})}{dt}=C_\frac{dU_c}{dt}}$, car $\boxed{q=C \times U_c}$ et $\boxed{\frac{dC}{dt}=0}$
	
	$$
	\begin{align*}U_c+(r\times i)+ (R \times i) &= E \\ U_c + i(r+R) &= E \\ U_c + \frac{dU_c}{dt}C(r+R)&= E \end{align*}
	$$
	1. Résoudre l’équation différentielle de façon à obtenir l’expression de $U_c(t)$
	
	$$
	\begin{align*} U_c + \frac{dU_c}{dt}C(r+R)&= E \\ \frac{dU_c}{dt}C(r+R) &= -U_c + E \end{align*}$$
	$$
	\begin{align*}\frac{dUc}{dt}&=-\frac{U_c}{C(r+R)}+\frac{E}{C(r+R)}\\ \frac{dUc}{dt}&=-\frac{1}{C(r+R)}\times U_c+\frac{E}{C(r+R)} 
	\end{align*}
	$$
	
	Or $y'=ay+b \Leftrightarrow y= K\times e^{ax}-\frac{b}a$
	
	$$
	\begin{align*} \frac{dUc}{dt}&=-\frac{1}{C(r+R)}\times U_c+\frac{E}{C(r+R)} \\ \space \\U_c &= K \times e^{-\frac{t}{C(r+R)}}+E \\ U_c(0) &= K \times e^0 +E \\ 0&= K+E \\-E &=K \\ \space \\ U_c &=-Ee^{-\frac{t}{C(r+R)}}+E \\U_c(t) &= E(1-e^{-\frac{t}{C(r+R)}}) \end{align*}
	$$
### _**Exercice 5 :**_

![[Physique-Chimie/6 Le condensateur et ses applications/Exercice 5.png]]
![[Cor_5.png]]
![[Cor_5_2.png]]

### _**Exercice 6 :**_

![[Physique-Chimie/6 Le condensateur et ses applications/Exercice 6.png]]
![[Cor_6.png]]
