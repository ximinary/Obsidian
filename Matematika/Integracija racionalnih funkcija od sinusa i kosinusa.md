#fax #math #a2 [deo poglavlja [[Neodređeni integral|"neodređeni integral"]]]

### Integrali oblika $\begin{align}\int R(\sin x,\,\cos x) \, dx \end{align}$, gde je $R$ racionalna funkcija od dva argumenta

- Ako je $R$ neparna po sinusu tj. važi $R(-\sin x,\, \cos x)=-R(\sin x,\,\cos x)$
  $\:$
  Radimo smenu $\begin{align}\binom{t=\cos x}{dt = -\sin x\,dx}\end{align}$
Tada, $\sin^{2}x=1-t^{2}$
$\:$
- Ako je $R$ neparna po kosinusu tj. važi $R(\sin x,\, -\cos x)=-R(\sin x,\,\cos x)$
  $\:$
Radimo smenu $\begin{align}\binom{t=\sin x}{dt = \cos x\,dx}\end{align}$
Tada, $\cos^{2}x=1-t^{2}$
$\:$
- Ako je $R$ parna po sinusu i kosinusu tj. važi $R(-\sin x,\, -\cos x)=R(\sin x,\,\cos x)$
  $\:$
Radimo smenu $\begin{align}\binom{t=\mathrm{tg}\, x\quad \Rightarrow\quad x = \mathrm{arctg}\,t}{dx = \frac{dt}{1\,+\,t^{2}}}\end{align}$, interval: $\begin{align}x\in\Big(\!-\!\frac{\pi}{2},\,\frac{\pi}{2}\Big)\end{align}$
$\:$
Tada, $\begin{align}\sin^{2} x=\frac{\sin^{2} x}{\cos^{2}x+\sin^{2} x}=\frac{\mathrm{tg}^{2}\,x}{1+ \mathrm{tg}^{2}\,x}=\frac{t^{2}}{1+t^{2}}\end{align}$
$\:$
$\quad\quad\ \ \begin{align}\cos^{2} x=\frac{\cos^{2} x}{\cos^{2}x+\sin^{2} x}=\frac{1}{1+ \mathrm{tg}^{2}\,x}=\frac{1}{1+t^{2}}\end{align}$
$\:$
- Ako ne važi nijedan od uslova gore radimo smenu $\begin{align}\binom{t=\mathrm{tg}\, \frac{x}{2}\quad \Rightarrow\quad x = 2\,\mathrm{arctg}\,t}{dx = \frac{2\,dt}{1\,+\,t^{2}}}\end{align}$, interval: $x\in(-\pi,\,\pi)$
$\:$
Tada, $\begin{align}\sin x=\frac{2\,\sin\frac{x}{2}\,\cos\frac{x}{2}}{\cos^{2}\frac{x}{2}+\sin^{2}\frac{x}{2}}=\frac{2\,\mathrm{tg}\,\frac{x}{2}}{1+ \mathrm{tg}^{2}\,\frac{x}{2}}=\frac{2\,t}{1+t^{2}}\end{align}$
$\:$
$\quad\quad\ \ \begin{align}\cos x=\frac{\cos^{2} \frac{x}{2}-\sin^{2}\frac{x}{2}}{\cos^{2}\frac{x}{2}+\sin^{2} \frac{x}{2}}=\frac{1- \mathrm{tg}^{2}\,\frac{x}{2}}{1+ \mathrm{tg}^{2}\,\frac{x}{2}}=\frac{1-t^{2}}{1+t^{2}}\end{align}$
