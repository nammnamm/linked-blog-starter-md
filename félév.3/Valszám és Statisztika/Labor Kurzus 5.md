L4 nél volt elutasítás modszere
(U,Y)->U<=f(Y)/cg(Y)->X1(az i edik x nek) = Y

varhatoan c darab parost generalunk


L5 közrefogás modszere

X szerkezi mintavételezhető folytonos valószínűségi változó ->f
U->U([0,1])
Y konnyu --||--
c>0 konstants
h1, h2 R-> R konnyen kiertekelheto tetsz fuggvenyek
0<=h1(x)<=f(x)<=h2(x)<=cg(x), barmely x eleme R

0<=h1(Yj)<=f(Yj)<=h2(Yj)<=cg(Yj)

ha Wj <= h1(Yj) gyors elfogadai tartomany

Wj >= h2(Yj) gyors elutasitasi tartomany

ha se h1 alatt se h2 felett akkor

h1(Yj) <=Wj<=h2(Yj)
Wj<=f(Yj)

{(Ui,Yj)}(j=1 N ig) parosok esetén

Uj cg(Yj)=:Wj
=>{(Wj,  Yj)}(j=1 N ig)

ezekrol volt rajz is fennebb a leirtakrol



h1, h2 also es felso becslofg ek


varhatoan hanyszor ertekeljuk ki az f et?

Nf=sum(j=1 tol N ig)1[also index h1(Yj)<Wj<h2(Yj)]

indikator fuggveny/ karakterisztikus fuggveny
1A(w)(A 1 nek alsó indexe)={0, W !eleme A
         1, w eleme A

multheti(4 het) P(X=B) =integral f(x) dx x eleme B
E(Nf) = E(N)(kicsi c 4 es laborbol)P(h1(Y1 eltunt a dzumma kitevoben alul akarmi lehet akar semmi is)<W1<h2(Y1)) = c P(h1(Y1)<W1<h2(Y1))= c integral(y eleme nagy omega )
(P(h1(Y1)<Ucg(Y1)<h2(Y1)|Y1=y)g(y)dy= c integral(y eleme nagy omega)(P(h1(y)<Ucg(y(<h2(y))g(y)dy= c integral(y eleme nagy omega)(h1(y)/Cg(y)<U<h2(y)/Cg(y))g(y)dy = c integral(y eleme nagy omega)F(lent U)[(h2(y)/Cg(y)- Fu(h1(y)/Cg(y))g(y)dy]= c integral y eleme nagy omega (h2(y)/Cg(y)-h1(y)/Cg(y)) gcxdy = integral y eleme nagy omega (h2(y)-h1(y)) dy

also es felso becslofg ek szerkesztese
Taylor-sorbafejtes
x0-pont körül
x0 = 0
f(x) = f(x0) + (x-x0)/1!f'(0) + (x2/2!)f''(0) +...

pl Cauchy g(x) = 1/pi(1+x^2) ez Y, x eleme R
c=sqrt(2pi/e)

X~N(0,1) f(x)=(1/sqrt(2pi))e^((-x^2)/2), x eleme R
e^(-x)=1 +x(-1)+ (x^2)/2!(1)+(x^3)/3!(-1)
x0=0+...= 1 - x + (x^2)/2 - (x^3)/6+...+
f(0)=1
f'(0)=-1
f''(0)=1


1-x<=e^(-x)<=1-x+(x^2)/2

e->(x^2)/2

e^(x^2/2) megkozelitoleg 1-x^2/2+(x^2/2)^2/2+...+1-(x^2)/2+(x^4)/8-(x^6)/48+....


W= Ucg(Y)=U c 1/(1+ Y negyzet) <= f(Y) =1/sqrt(2pi)szor e ^(-(Y^2)/2) osztott sqrt 2pi vel 2 szer talán
a vége 
U szor pi/sqrt(e) szor 1/(1/2 + (Y^2)/2) <=e-Y2/2

1/2 beta
S az (Y^2)/2

W=(alfaU)/(beta + S)

sqrt 2 pi f(Y) egyenlo e a minusz S edikenen

sqrt 2 pi h1(Y) egyenlo 1 minusz S (minusz sqrt2, sqrt2)

h2 szor cg -> c

ez mind benne van pdf szopas