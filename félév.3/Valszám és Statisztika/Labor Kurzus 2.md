elemi eseményke és azok tere
kisérlet
{wi}(i eleme I) = nagy omega
Eseményalgebra
Valószínűség axiomatikus értelmezése

 Szigmaalgenra kiegeszitve .....

Minden esemenybeli mezonek .. az (nagy omega, A, P) Az omega mondja .eg hogy ez véges v végtelen

pl kocka
{1, 2, 3, 4, 5, 6}

> ==================~~[[********]()]()~~~~~~~~~~~~==================



szigmaalgebran beluli dolgokat tudom merni a A, P vel

		- [x] ![[![[#]]]]

Diszkrét valoszinusegi valtozo amikor omega véges vagy legfeljebb megszamlalhatoan vegtelen hosszusagu


folytonos: omega kontinuum szamossagu
.

Diszkrét:
		pl kocka (1 2 3 4 5 6)
			(1/6 1/6 1/6 1/6 1/6 1/6) U(6)



		Binomiális Bino(n, p) n- ismétlések száma n eleme N
		p- a vizsgált eset bekövetkezése val- e o eleme (0, 1)
		(k)
		(C(n)(k)p^k(1-p)^n-k)k=0,n
		n húzásból k db párost húztam
		
k db piros
piros feher piros ... piros ... piros feher
p.        1-p.     p.         m-k db.  p.       1-p


Geometriai Geo(p) p eleme (0,1)
(k)
|k-1|
((1-p)p)k>=1

eloszlásfg {F(lent X):R->R
{F(X lent)(x)=P(X < x)•

F(X lent)(-2) = P(X<-2) = 0(lehetetlen esemeny)
F(X lent)(7) = P(X<7) = 1
F(X lent)(3,2) = P(X=1) +P(X=2) + P(X=3)1/6+1/6+1/6=1/2

lépcsőzetes rajzika F ig
matlabban • van implementálva
Diszkrét esetben mindig lépcsős fgv
relatív gyakoriság a kicsi f


Folytonos eloszlások példa:


egyenletes U([a,b])

f(x)(lent U([a, b])) = {1/b-a , x eleme [a, b]
			    { 0, x nem eleme [a, b]


rajzika


F(X)(x)= integrál ( - vegtelentol x ig) (f(lentX)(t)dt)

integral nx(1/b-a) dt = 1/b-a t |nx. = x-a / b-a


	F(X lent)(x) = {0, x< a
			{x-a/b-a, x eleme [a, b]
			{1, x> b



hosszu pdf 57


Nevezetes diszkrét valószínűségi változók

suruseg es eloszlasfgv

cdg valtozatok eloszlasfuggvenyt kell kiszamolna am
a cdf fuggvenyek teljesen uresek


a discrete az osszegzes a folytonos integralas

a discrete esetet leimtegrál.hogy folytonos kegyen csak simán lecserél operátor a discreteket megirjuk itt otthon lemasol s kicserel integralra

s megnezunk 1 peldat s az alapjan meg lehet csinalni


kell tesztállomány saját eloszlásra s ráhív plot a tesztet is itt megírjuk s majd átírjuk arra 

discrete cfd felir ami a fejlécén kívűl üres

function F = DiscreteCDF(x, distribution_type, parameters)

(ez egy alias)f = @(x) DiscreteCDF(x, distribution_type, parameters);
n= length(x);
F = zeros(1, n);
x_min = 0;


switch distribution_type
		case 'geometric'
			x_min = 1;
end(ha valami más lesz akkor át kell írni itt valamit)

F(1) = sum(f(x_min:x(1)));

for i = 2: n
	F(i) = F(i-1) + sum(f(x(i-1)+1:x(i)));
end
end



tesztallomany

function testDiscrete
x = [1:8];
p= 0,33
distribution_type = 'geometric';
parameters = p;
f = DiscretePDF(x, distribution_type, parameters);
subplot 1 2 1
plot x f .g
hold on
plot(x, F, 'r') stairs parancs hogy lepcsoket rajzoljon, kulonben osszekoti akkoris ha leocsozetes a sima plot
ff = geopdf(x,p)
FF = geocdf prrrttt
plot x ff .g
subplot 1 2 2
end


1 tol van nalunk a geomegriai angolban 0 tol csak a geometriainal van igy azt akarjuk egymas melle keruljon a 2 abra subplot paranccsal
1x2 rajz 1 sor 2 cella egyik cella sajat a masik cella matlabé subplot(1,2,1); 1x2 felosztas 1 be rajzolja a sajat kodban benne van hogyan kell hivatkozni rájuk


cdf be elvileg nem kell belenyulni binomialisnal de a pdf nel kell teszt

continousos cdf discretecdf peldajara a for on belul sum ot integralra cserel beallit a megfelelo min ertek es minden sum ot integralra cserel
nem discretet hanem continuous t hív

belelehet infinityt írni most az integrálba de a 3. feladat 50/57 nel nem kell quad fgv

surusegfgv, relativ gyakorisag fgv

plusszfeladat gg
táblázat alapján oldd feladat

leimplementál minden 


pluszfeladat 2 is van papiros számolást hoz, canvasre kell feltölteni
következő hétfői óráig kell feltölteni és azon a héten laboron be lehet mutatni azt
bescannel papír s mellé minden használt kód, számolás is

4. feladat diszkrét eloszlás sikidom amin belul a kulonbozo szamok 10 ertekey felvevo valoszinusegi valtozo, az adott terulet arany tartozik ezt kell papiron felirni ,  legeloszor felir milyen ertekek tartoznak hozza mimt a kockanal es meghataroz eloszlasfgv es annak a képletet , ha ez megvan akkor a 3 esemény valószínűsége ezeket papiron kiszámol, elég tört alakban, átmegy utanna matlabba discrete pdf et kiegeszit ezzel az eloszlas tablazattal es elkeszit peldat discrete pdf es cdf altal es kiszamol valosinusegi ertek kodban is
5. folytonos eloszlás esetben papiron minden surusegfgv egysegnyi terulettel rendelkezik s nem negativ az alfa szamitasnal integral a teljes elven 3 ag integraljanak osszege 1 kell legyen alfatol kellene fuggjon = tesz 1 el ezutan kiszamol papiron eloszlasfgv papiron kell integralni utanna a pdf ben levo ertekekre kiszamol eloszlasfgv pdf ben benne van kulonbozo dolgok valoszinuseg
6. kiegeszit continuous pdf es cdf ujabb case ág és ír teszt ezekre is ha ez megvan kiszamol az adott esetekre, ha helyesen számolt akkor a papiros érték megeggyezik a kódossal feltolt continuous pdf cdf rs discrete cdf pdf es tesztallomanyok
jovohetre mar elso 2 feladat 