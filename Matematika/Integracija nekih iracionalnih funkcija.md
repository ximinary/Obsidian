#fax #math #a2 [deo poglavlja [[Neodređeni integral|"neodređeni integral"]]]

##### Integral oblika $\begin{align}\int R\left( x,\,\sqrt[n]{\frac{ax+b}{cx+k}} \right) \, dx \end{align}$,
gde je $R$ racionalna funkcija od dva argumenta, rešavamo smenom
$\begin{align}\left(\begin{array}{}{t=\sqrt[n]{\frac{ax+b}{cx+k}}\quad\Rightarrow\quad t^{n}=\frac{ax+b}{cx+k}\quad\Rightarrow\quad x=\frac{b-kt^{n}}{ct^{n}-a}}\\{dx=\frac{(ak-bc)\,n\,t^{n-1}}{(ct^{n}-a)^{2}}dt} \end{array}\right)\end{align}$ i dobijamo [[Integracija racionalnih funkcija|integral od racionalne funkcije]].

##### Smene za oslobođenje od korena
1. $\begin{align}\int \sqrt[]{1-x^{2}} \, dx &=\binom{x=\sin t}{dx=\cos t\, dt}=\int \sqrt[]{1-\sin^{2}t}\, \cos t\, dt=\int |\cos t|\cos t \, dt=\dots\end{align}$
2. $\begin{align}\int \sqrt[]{x^{2}-1} \, dx &=\binom{x=\frac{1}{\sin t}}{dx=-\frac{\cos t}{\sin^{2}t}\, dt}=\int \sqrt[]{\frac{1}{\sin^{2} t}-1}\bigg(\!\!-\frac{\cos t}{\sin^{2}t}\bigg)\, dt=-\int \left|\frac{\cos t}{\sin t}\right|\,\frac{\cos t}{\sin^{2}t} \, dt=\dots\end{align}$
3. $\begin{align}\int \sqrt[]{1+x^{2}} \, dx &=\binom{x=\mathrm{tg\,}t}{dx=\frac{dt}{\cos^{2}t}}=\int \sqrt[]{\frac{\sin^{2} t}{\cos^{2} t}+1}\,\frac{1}{\cos^{2}t}\, dt=\int \left|\frac{1}{\cos t}\right|\,\frac{1}{\cos^{2}t} \, dt=\dots\end{align}$

##### Integral oblika $\begin{align}\int R(x,\,\sqrt[]{ax^{2}+bx+c}) \, dx \end{align}$,
gde je $R$ racionalna funkcija od dva argumenta, rešavamo nekim od sledećih metoda:
- **Mnogo smena:**
  Dopunjamo do kvadrata binoma:
  $\begin{align}\sqrt[]{ax^{2}+bx+c}=\sqrt[]{\mathrm{sgn}\,a\bigg(\Big(\underbrace{\sqrt[]{|a|}x+\frac{b}{2\sqrt[]{|a|}}}_{=\,t}\Big)^{2}\underbrace{-\frac{b^{2}}{4a}+c}_{=\,\alpha\,\in\,\mathbb{R}}\bigg)}=\sqrt[]{ \mathrm{sgn}\,a\,(t^{2}+\alpha)}\end{align}$
  još jednom smenom $\begin{align}u = \frac{t}{\sqrt[]{|\alpha|}}\end{align}$ dobijamo $\sqrt[]{|\alpha|}\,\sqrt[]{1-u^{2}},\ \sqrt[]{|\alpha|}\,\sqrt[]{u^{2}-1}\,$ ili $\sqrt[]{|\alpha|}\,\sqrt[]{1+u^{2}}$, što dalje rešavamo trigonometrijskom smenom iz [[Integracija nekih iracionalnih funkcija#Smene za oslobođenje od korena|odeljka gore]] — dobijamo integral [[Integracija racionalnih funkcija od sinusa i kosinusa|oblika]] $\begin{align}\int R_{1}(\sin s,\,\cos s) \, ds \end{align}$
$\:$
- **I Ojlerova smena**, ako $a>0$
  $\sqrt[]{ax^{2}+bx+c}=\pm\sqrt[]{a}\,x\pm t$
  $\cancel{ax^{2}}+bx+c=\cancel{ax^{2}}\pm2\sqrt[]{a}\,x\,t+t^{2}$
  $x= \frac{t^{2}-c}{b\mp2\sqrt[]{a}\,t}\quad\Rightarrow\quad dx=\cdot\!\cdot\!\cdot\, dt$
$\:$
- **II Ojlerova smena**, ako $c>0$
$\sqrt[]{ax^{2}+bx+c}=\pm\, x\,t\pm \sqrt[]{c}$
  $ax^{2}+bx+\cancel{c}=x^{2}\,t^{2}\pm2\sqrt[]{c}\,x\,t+\cancel{c}\quad\Big|:x$
  $ax+b=x\,t^{2}\pm2\sqrt[]{c}\,t$
  $x= \frac{b\mp2\sqrt[]{c}\,t}{t^{2}-a}\quad\Rightarrow\quad dx=\cdot\!\cdot\!\cdot\, dt$
$\:$
- **III Ojlerova smena**, ako $D\geqslant0$ 
 $\quad\quad$ Neka su $x_{1},\,x_{2}\in\mathbb{R}$ koreni polinoma,
 $\quad\quad$ tada $ax^{2}+bx+c=a(x-x_{1})(x-x_{2})$
 $\:$
$\sqrt[]{ax^{2}+bx+c}=t(x-x_{1})$
  $a(x-x_{1})(x-x_{2})=t^{2}(x-x_{1})^{2}\quad\Big|:(x-x_{1})$
  $ax-ax_{2}=t^{2}x-t^{2}x_{1}$
  $x= \frac{t^{2}x_{1}-ax_{2}}{t^{2}-a}\quad\Rightarrow\quad dx=\cdot\!\cdot\!\cdot\, dt$
  