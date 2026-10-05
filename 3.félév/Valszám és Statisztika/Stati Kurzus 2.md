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