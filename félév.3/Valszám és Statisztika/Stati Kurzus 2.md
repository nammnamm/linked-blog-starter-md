Valoszinuség tulajd:
(nagy omega, K P)
Ért: P:K -> R
     P(nagy omega) = 1
     P(A)>=0
     P(U(i 1 tol n ig)Ai) = Sum(1 tol n igP(Ai)), ha Ai metszve P, i,j eleme {1,...,n}.

Tulajd: a) P(nem letezo esemeny) =0
Biz: nagy omega = nagy omega U nem letezo esemeny
nagy omega metszve lehetetlen esemeny = lehetetlen esemeny
     =>P(nagy omega)= P(nagy omega U lehetetlen esemeny)= P(nagy omega) + P(lehetetlen esemeny) => P(lehetetlen esemeny)
     b) P(!A) = 1- P(A)
     Biz: A U !A = nagy omega
     A metszve !A = lehetetlen esemeny => P(A U !A) =1 P(A) + P(!A) =1
     c) P(B\A) = P(B) - P(B metszve A)
     biz. (B\A)metszve(B netszve A)= lehetetlen esemeny
     d) A implikálja B => P(A)<=P(B)
     Biz B metszve A = A
     P(B)- P(A) = P(B\A)>=0
     e)P(AUB) = P(A) + P(B) - P(A metszve B)
     Biz  A U ( B\A)
     A metszve (B\A) = lehetetlen esemeny
     P(AUB)=P(A) + P(B\A) = P(A) + P(B) - P(A metszve B)
     f) (Ai)(lent i=1,n)   P(U(i 1 tol n ih)Ai) = sum(i tol n ig)P(Ai) - sum(i,j 1 tol n ig)P(Ai metszve Aj)+...+ -1^(n+1)P(metszetjel 1 tol n ig)Ai
     Biz.    n = 2
     felt n
     biz n+ 1
     P(U(1 tol n ig)Ai U An+1)= P(U(1 tol n ih)Ai) + P(An+1) - P((U(1 tol n ig )Ai) metszve An+1) = sum(1 tol n ig) P(Ai) - sum(i,j 1 tol n ig)P(Ai metszve Aj) + ... + (-1)^(n+1).  P(metszet(1 tol n ig)Ai) + P(An+1) - [sum(1 tol n ig i)P(Ai metszve An+1)- sum(i,j 1 tol n ig)P(Ai metszve Aj metsve An+1) + ... (-1)^n+1P(metszve(i 1 tol n ig)Ai metszve An+1)]. = sum(1 tol n ig)P(Ai) - sum(i,j 1 tol n ig)P(Ai metszve Aj) +...+ (-1)^n+1P(metszve(i 1 tol n+1)Aj)
Valószínűség : - klasszikus(relatív gyakoriság)
             -diszkrét
             -geometriai P(A)= nu(A)/nu(nagy omega)

d hossz az egyenesek kozott l a tű hossza s meg kell határozni hogy ráesik e
______
______
______
nagy omega = {(X, alfa)| 0<=alfa<=pi, 0<=x<=l/2}
nu(nagy omega) = (pi szor d)/2
A={x, alfa| 0<=alfa<=pi, 0<=x<=l/2 szor sin alfa}
integrálással kell kiszámolni a várt területet
nu(A) = integrál(l/2 sin alfa d alfa) = l
P(A) = 2l/(pi szor d) megközelítőleg k/n

4 edik Feltételes valószínűség
(nagy omega, K, P)
B eleme K : P(B)>0
P(A|B) = P(A metszve B)/ P(B) jelölés P(A) alatta B

fg. val
     P(A|B) >= 0
     P(nagy omega | B) = P(nagy omega metszve B)/ P(B)= P(B)/P(B) = 1
     P(U(1 tol n ig)Ai|B) = P((U(1 tol nig )Ai)metszve B)/ P( B) = P(U(1tol n ig)(Ai metszve B))/ P(B) = sum( 1 tol n ig)P(Ai metszve B)/P(B) = sum( 1 tol n ig)P(Ai|B)

Tulajd:
a).    P(A metszve B) = P(A|B)P(B)
b).    P(metszve(i 1 tol n ig)Ai)= P(A1)P(A2|A1)P(A3|A1 metszve A2) .... P(An|A1 metszve ..... metszve An-1)

Biz: P(A1). P(A2 metszve A1)/P(A1). P(A3 metszve A1 metszve A2)/P(A1 metszve A2).  .... P(metszve(1 tol n ig)Ai)/P(metszve(1 tol n ig)A j)

c) TELJES VALÓSZÍNŰSÉG TÉTELE 
(Ai)(lent i= 1 tol n ig) t.e. rendszer : U( i 1 tol n ig)Ai = nagy omega
Ai metszve Aj = lehetetlen esemeny, barmely i,j eleme {1,...,n}
(Ai)(lent i = 1,n) t.e.r( teljes esemény rendszer tétele)
A eleme K
P(A)= sum(1 tol n ig)P(A|Ai)P(Ai)

Biz:   U(1 tol n ig)Ai = nagy omega
     A netszve nagy omega = A = A metszve (U(1 tol n ig)Ai) = U(1 tol n ig)(A metszve Ai)
     (A metszve Ai) metszve (A metszve Aj) = lehetetelen esemény, i!= j
     P(A) - P(U(1 tol n ig)(A metszve Ai)) = sum( 1 tol n ig)P(A metszve Ai) = sum(1 tol n ig)P(A|Ai)P(Ai)

     d)Bayes tétele!!!!
     (Ai)(lent i = 1,n) t.e r A eleme K
 P(Ai|A) = (P(A|Ai)P(Ai))/(sum(1 tol n ig)P(A|Aj)P(Aj))
LESZ SZÓBELI VIZSGÁN SZÓBELI
Biz: P(Ai|A) = P(Ai metszve A)/ P(A) = (P(A|Ai)P(Ai))/sum(1 tol n ig)P(A|Aj)P(Aj)

Események függetlensége:
     A,B:     P(A metsze B) = P(A)P(B)
     (Ai)(1 tol n ig) - páronként P(Ai metszve Aj) = P(Ai)P(Aj), barmeky i,j eleme { 1,...,n} i!=j
     -teljesen függetlenek.  P(metszve(1 tol l ig)Ai) = szogletes metszet(1 tol l' ig)P(Ai)
PLUSZPONT. Ha egy esemény valószínűsége 1 az a biztos esemény? 5 pontos kérdés következő órára PLUSZPONT

ha teljesen fuggetlen akkor páronként is az de fordítva nem igaz

nagy omega = {w1, w2, w3, w4}
A1 = {w1, w4}
A2 = {w2, w4}
A3 = {w3, w4}.       vizsgálják meg mi történik



Valószínűségi modellek:
           Bernoulli visszatevéssel 2 állapottal(Binomiális modell)

A valószínűség P(A)=p.  P(!A)a = 1-p = q
n ismétlés mi annak a valószínűsége hogy k szor bekovetkezett és n-k szor nem

n- ism kszor A, n-k szor !A

urna A fehér golyó B lila golyó

a/a+b. ez. p.  b/a+b.   ez 1-p

B(lent n,k)  = U[A(lent i1) metszet Ai2 metszet .... metszet Aik metszet !Aik+1 metszve .... metszve !Ain]

1<=i1<i2<....<ik<=n

P(Bn,k) = sum P(Ai1 metszve ... metszve Ai2 metszve !Aik+1 metszve ...metszve !Ain)
[Ai1 metszve .... metszve Aik metszve !Aik+1 metszve ... !Ain] metszve [Aj1 metszve ... metszve Ajk metszve !Ajk+1 metszve .... metszve Ajn] = lehetetlen esemény

valamiért a fenti metszetek a bernoulli mák és el volt mondva szóban de a jele metszet votlt


P(Bn,k) = sum P(A1)... P(Ak)(idaig p^k)P(!Ak+1) ... P(!An)(a masiktol idaig q^(n-k))  =Cnk p^k q^(n-k)


Megj.    sum(k=0 tol n ig)P(Bn,k) = (p+q)^n=1

(Bn,k)(k=0,n) t.e.r.                   U(k=0 tol n ig)Bn,k = nagy omega