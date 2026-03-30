# First homework question

## Commonly Asked Questions in First-Order ODE (20 questions)

### Separable variables

**① 題目：** $\frac{dy}{dx} = xy$

$$\begin{aligned}
\frac{1}{y} dy &= x dx \\
\int \frac{1}{y} dy &= \int x dx \\
\ln|y| &= \frac{1}{2}x^2 + C_1 \\
y &= C e^{\frac{1}{2}x^2}
\end{aligned}$$

**② 題目：** $\frac{dy}{dx} = \frac{x}{1+y^2}$

$$\begin{aligned}
(1+y^2) dy &= x dx \\
\int (1+y^2) dy &= \int x dx \\
y + \frac{1}{3}y^3 &= \frac{1}{2}x^2 + C
\end{aligned}$$

**③ 題目：** $(1+y)e^{-x}dx + dy = 0$

$$\begin{aligned}
dy &= -(1+y)e^{-x} dx \\
\int \frac{1}{1+y} dy &= \int -e^{-x} dx \\
\ln|1+y| &= e^{-x} + C_1 \\
1+y &= C e^{e^{-x}} \Rightarrow y = C e^{e^{-x}} - 1
\end{aligned}$$

**④ 題目：** $\frac{dy}{dx} = y\ln y$

$$\begin{aligned}
\frac{1}{y\ln y} dy &= dx \\
\int \frac{1}{\ln y} d(\ln y) &= \int dx \\
\ln|\ln y| &= x + C_1 \\
\ln y &= C e^x \Rightarrow y = e^{C e^x}
\end{aligned}$$

### 二、Linear differential equations

**⑤ 題目：** $y' + 2y = e^{-x}$

$$\begin{aligned}
I.F. &= e^{\int 2 dx} = e^{2x} \\
e^{2x}y' + 2e^{2x}y &= e^x \\
(e^{2x}y)' &= e^x \\
e^{2x}y &= e^x + C \\
y &= e^{-x} + C e^{-2x}
\end{aligned}$$

**⑥ 題目：** $y' - y = x$

$$\begin{aligned}
I.F. &= e^{\int -1 dx} = e^{-x} \\
(e^{-x}y)' &= x e^{-x} \\
e^{-x}y &= \int x e^{-x} dx = -x e^{-x} - e^{-x} + C \\
y &= -x - 1 + C e^x
\end{aligned}$$

**⑦ 題目：** $y' + 3y = 6, \quad y(0)=1$

$$\begin{aligned}
I.F. &= e^{3x} \\
(e^{3x}y)' &= 6e^{3x} \\
e^{3x}y &= 2e^{3x} + C \\
y &= 2 + C e^{-3x} \\
y(0) &= 2 + C = 1 \Rightarrow C = -1 \\
y &= 2 - e^{-3x}
\end{aligned}$$

**⑧ 題目：** $y' + y = e^{2x}$

$$\begin{aligned}
I.F. &= e^x \\
(e^xy)' &= e^{3x} \\
e^xy &= \frac{1}{3}e^{3x} + C \\
y &= \frac{1}{3}e^{2x} + C e^{-x}
\end{aligned}$$

**⑨ 題目：** $x\frac{dy}{dx} + y = x^2$

$$\begin{aligned}
\frac{dy}{dx} + \frac{1}{x}y &= x \\
I.F. &= e^{\int \frac{1}{x} dx} = x \\
(xy)' &= x^2 \\
xy &= \frac{1}{3}x^3 + C \\
y &= \frac{1}{3}x^2 + \frac{C}{x}
\end{aligned}$$

### 三、Bernoulli equation

**⑩ 題目：** $y' + y = xy^2$

$$\begin{aligned}
y^{-2}y' + y^{-1} &= x \\
\text{Let } u &= y^{-1}, \ u' = -y^{-2}y' \\
-u' + u &= x \Rightarrow u' - u = -x \\
I.F. &= e^{-x} \\
(e^{-x}u)' &= -x e^{-x} \\
e^{-x}u &= x e^{-x} + e^{-x} + C \\
u &= x + 1 + C e^x \\
y &= \frac{1}{x + 1 + C e^x}
\end{aligned}$$

**⑪ 題目：** $y' - 2y = e^x y^3$

$$\begin{aligned}
y^{-3}y' - 2y^{-2} &= e^x \\
\text{Let } u &= y^{-2}, \ u' = -2y^{-3}y' \\
-\frac{1}{2}u' - 2u &= e^x \Rightarrow u' + 4u = -2e^x \\
I.F. &= e^{4x} \\
(e^{4x}u)' &= -2e^{5x} \\
e^{4x}u &= -\frac{2}{5}e^{5x} + C \\
u &= -\frac{2}{5}e^x + C e^{-4x} \\
y^{-2} &= -\frac{2}{5}e^x + C e^{-4x}
\end{aligned}$$

**⑫ 題目：** $xy' + y = y^2$

$$\begin{aligned}
y' + \frac{1}{x}y &= \frac{1}{x}y^2 \\
y^{-2}y' + \frac{1}{x}y^{-1} &= \frac{1}{x} \\
\text{Let } u &= y^{-1}, \ u' = -y^{-2}y' \\
-u' + \frac{1}{x}u &= \frac{1}{x} \Rightarrow u' - \frac{1}{x}u = -\frac{1}{x} \\
I.F. &= e^{-\int \frac{1}{x} dx} = x^{-1} \\
\left(\frac{u}{x}\right)' &= -\frac{1}{x^2} \\
\frac{u}{x} &= \frac{1}{x} + C \Rightarrow u = 1 + Cx \\
y &= \frac{1}{1 + Cx}
\end{aligned}$$

### 四、Exact Equation

**⑬ 題目：** $(2xy+y^2)dx + (x^2+2xy)dy = 0$

$$\begin{aligned}
M_y &= 2x+2y, \quad N_x = 2x+2y \quad (\text{Exact}) \\
\int M dx &= x^2y + xy^2 + g(y) \\
\frac{\partial}{\partial y}(x^2y + xy^2 + g(y)) &= x^2 + 2xy + g'(y) = N = x^2 + 2xy \\
g'(y) &= 0 \Rightarrow g(y) = C \\
x^2y + xy^2 &= C
\end{aligned}$$

**⑭ 題目：** $(y\cos x + 2x)dx + (\sin x + 3y^2)dy = 0$

$$\begin{aligned}
M_y &= \cos x, \quad N_x = \cos x \quad (\text{Exact}) \\
\int M dx &= y\sin x + x^2 + g(y) \\
\frac{\partial}{\partial y}(y\sin x + x^2 + g(y)) &= \sin x + g'(y) = N = \sin x + 3y^2 \\
g'(y) &= 3y^2 \Rightarrow g(y) = y^3 \\
y\sin x + x^2 + y^3 &= C
\end{aligned}$$

**⑮ 題目：** $(y+x^2)dx + (x+y^2)dy = 0$

$$\begin{aligned}
M_y &= 1, \quad N_x = 1 \quad (\text{Exact}) \\
\int M dx &= xy + \frac{1}{3}x^3 + g(y) \\
\frac{\partial}{\partial y}\left(xy + \frac{1}{3}x^3 + g(y)\right) &= x + g'(y) = N = x + y^2 \\
g'(y) &= y^2 \Rightarrow g(y) = \frac{1}{3}y^3 \\
xy + \frac{1}{3}x^3 + \frac{1}{3}y^3 &= C_1 \Rightarrow x^3 + y^3 + 3xy = C
\end{aligned}$$

### 五、Homogeneous equations

**⑯ 題目：** $\frac{dy}{dx} = \frac{x+y}{x}$

$$\begin{aligned}
y' &= 1 + \frac{y}{x} \\
\text{Let } y &= ux, \ y' = u + xu' \\
u + xu' &= 1 + u \\
xu' &= 1 \Rightarrow du = \frac{1}{x} dx \\
u &= \ln|x| + C \\
\frac{y}{x} &= \ln|x| + C \\
y &= x\ln|x| + Cx
\end{aligned}$$

**⑰ 題目：** $\frac{dy}{dx} = \frac{x^2+y^2}{xy}$

$$\begin{aligned}
y' &= \frac{x}{y} + \frac{y}{x} \\
\text{Let } y &= ux, \ y' = u + xu' \\
u + xu' &= \frac{1}{u} + u \\
xu' &= \frac{1}{u} \Rightarrow u du = \frac{1}{x} dx \\
\frac{1}{2}u^2 &= \ln|x| + C_1 \\
\frac{1}{2}\left(\frac{y}{x}\right)^2 &= \ln|x| + C_1 \\
y^2 &= 2x^2\ln|x| + C x^2
\end{aligned}$$

---

## Second-order ordinary differential equations(ODEs)-past exam questions TOP20

### 一、Characteristic Equation with Constant Coefficients

**① 題目：** $y'' - 5y' + 6y = 0$

$$\begin{aligned}
r^2 - 5r + 6 &= 0 \\
(r-2)(r-3) &= 0 \\
y &= C_1 e^{2x} + C_2 e^{3x}
\end{aligned}$$

**② 題目：** $y'' + 4y' + 4y = 0$

$$\begin{aligned}
r^2 + 4r + 4 &= 0 \\
(r+2)^2 &= 0 \\
y &= C_1 e^{-2x} + C_2 x e^{-2x}
\end{aligned}$$

**③ 題目：** $y'' + 9y = 0$

$$\begin{aligned}
r^2 + 9 &= 0 \Rightarrow r = \pm 3i \\
y &= C_1 \cos(3x) + C_2 \sin(3x)
\end{aligned}$$

**④ 題目：** $2y'' + 3y' - 2y = 0$

$$\begin{aligned}
2r^2 + 3r - 2 &= 0 \\
(2r-1)(r+2) &= 0 \\
y &= C_1 e^{\frac{1}{2}x} + C_2 e^{-2x}
\end{aligned}$$

**⑤ 題目：** $y'' - y = 0, \quad y(0)=1, \ y'(0)=0$

$$\begin{aligned}
r^2 - 1 &= 0 \Rightarrow r = \pm 1 \\
y &= C_1 e^x + C_2 e^{-x} \\
y' &= C_1 e^x - C_2 e^{-x} \\
y(0) &= C_1 + C_2 = 1 \\
y'(0) &= C_1 - C_2 = 0 \Rightarrow C_1 = \frac{1}{2}, C_2 = \frac{1}{2} \\
y &= \frac{1}{2}e^x + \frac{1}{2}e^{-x} = \cosh x
\end{aligned}$$

### 二、Non-homogeneous equations

**⑥ 題目：** $y'' - 3y' + 2y = e^x$

$$\begin{aligned}
y_h: r^2 - 3r + 2 &= 0 \Rightarrow r=1, 2 \Rightarrow y_h = C_1 e^x + C_2 e^{2x} \\
y_p &= A x e^x \\
y_p' &= A e^x + A x e^x, \quad y_p'' = 2A e^x + A x e^x \\
(2A+Ax)e^x - 3(A+Ax)e^x + 2Axe^x &= e^x \\
-A &= 1 \Rightarrow A = -1 \\
y &= C_1 e^x + C_2 e^{2x} - x e^x
\end{aligned}$$

**⑦ 題目：** $y'' + y = x^2$

$$\begin{aligned}
y_h &= C_1 \cos x + C_2 \sin x \\
y_p &= Ax^2 + Bx + C \Rightarrow y_p'' = 2A \\
2A + (Ax^2 + Bx + C) &= x^2 \\
A=1, \ B=0, \ 2A+C&=0 \Rightarrow C=-2 \\
y &= C_1 \cos x + C_2 \sin x + x^2 - 2
\end{aligned}$$

**⑧ 題目：** $y'' + 4y = \cos 2x$

$$\begin{aligned}
y_h &= C_1 \cos 2x + C_2 \sin 2x \\
y_p &= x(A \cos 2x + B \sin 2x) \\
y_p'' + 4y_p &= -4A \sin 2x + 4B \cos 2x = \cos 2x \\
A &= 0, \ B = \frac{1}{4} \\
y &= C_1 \cos 2x + C_2 \sin 2x + \frac{1}{4}x \sin 2x
\end{aligned}$$

**⑨ 題目：** $y'' + y = \sin x$

$$\begin{aligned}
y_h &= C_1 \cos x + C_2 \sin x \\
y_p &= x(A \cos x + B \sin x) \\
y_p'' + y_p &= -2A \sin x + 2B \cos x = \sin x \\
A &= -\frac{1}{2}, \ B = 0 \\
y &= C_1 \cos x + C_2 \sin x - \frac{1}{2}x \cos x
\end{aligned}$$

**⑩ 題目：** $y'' - y = e^x + x$

$$\begin{aligned}
y_h &= C_1 e^x + C_2 e^{-x} \\
y_p &= A x e^x + Bx + C \\
y_p'' - y_p &= 2A e^x - Bx - C = e^x + x \\
A &= \frac{1}{2}, \ B = -1, \ C = 0 \\
y &= C_1 e^x + C_2 e^{-x} + \frac{1}{2}x e^x - x
\end{aligned}$$

### 三、Variation of Parameters

**⑪ 題目：** $y'' + y = \tan x$

$$\begin{aligned}
y_1 &= \cos x, \ y_2 = \sin x, \ W = 1 \\
y_p &= -\cos x \int \sin x \tan x dx + \sin x \int \cos x \tan x dx \\
y_p &= -\cos x (\ln|\sec x + \tan x| - \sin x) - \sin x \cos x \\
y_p &= -\cos x \ln|\sec x + \tan x| \\
y &= C_1 \cos x + C_2 \sin x - \cos x \ln|\sec x + \tan x|
\end{aligned}$$

**⑫ 題目：** $y'' - y = e^{2x}$

$$\begin{aligned}
y_1 &= e^x, \ y_2 = e^{-x}, \ W = -2 \\
y_p &= -e^x \int \frac{e^{-x} e^{2x}}{-2} dx + e^{-x} \int \frac{e^x e^{2x}}{-2} dx \\
y_p &= \frac{1}{2}e^x \left(\frac{1}{2}e^{2x}\right) - \frac{1}{2}e^{-x} \left(\frac{1}{3}e^{3x}\right) = \frac{1}{12}e^{2x} \\
y &= C_1 e^x + C_2 e^{-x} + \frac{1}{3}e^{2x}
\end{aligned}$$

**⑬ 題目：** $y'' + 4y = \sec^2 2x$

$$\begin{aligned}
y_1 &= \cos 2x, \ y_2 = \sin 2x, \ W = 2 \\
y_p &= -\cos 2x \int \frac{\sin 2x \sec^2 2x}{2} dx + \sin 2x \int \frac{\cos 2x \sec^2 2x}{2} dx \\
y_p &= -\frac{1}{4}\cos 2x \sec 2x + \frac{1}{4}\sin 2x \ln|\sec 2x + \tan 2x| \\
y &= C_1 \cos 2x + C_2 \sin 2x - \frac{1}{4} + \frac{1}{4}\sin 2x \ln|\sec 2x + \tan 2x|
\end{aligned}$$

### 四、Euler–Cauchy equation

**⑭ 題目：** $x^2y'' + 3xy' + y = 0$

$$\begin{aligned}
\text{Let } y &= x^r \\
r(r-1) + 3r + 1 &= 0 \Rightarrow (r+1)^2 = 0 \\
y &= C_1 x^{-1} + C_2 x^{-1} \ln x
\end{aligned}$$

**⑮ 題目：** $x^2y'' - xy' + y = 0$

$$\begin{aligned}
r(r-1) - r + 1 &= 0 \Rightarrow (r-1)^2 = 0 \\
y &= C_1 x + C_2 x \ln x
\end{aligned}$$

**⑯ 題目：** $x^2y'' + xy' - y = x^2$

$$\begin{aligned}
r(r-1) + r - 1 &= 0 \Rightarrow r^2 - 1 = 0 \Rightarrow r = \pm 1 \\
y_h &= C_1 x + C_2 x^{-1} \\
y'' + \frac{1}{x}y' - \frac{1}{x^2}y &= 1 \Rightarrow f(x) = 1, \ W = -\frac{2}{x} \\
y_p &= -x \int \frac{x^{-1} \cdot 1}{-2/x} dx + x^{-1} \int \frac{x \cdot 1}{-2/x} dx = \frac{x^2}{3} \\
y &= C_1 x + C_2 x^{-1} + \frac{x^2}{3}
\end{aligned}$$

### 五、Order reduction method

**⑰ 題目：** 已知 $y_1=e^x$，求 $y'' - 2y' + y = 0$ 之第二解

$$\begin{aligned}
P(x) &= -2 \Rightarrow e^{-\int -2 dx} = e^{2x} \\
y_2 &= y_1 \int \frac{e^{-\int P(x) dx}}{y_1^2} dx \\
y_2 &= e^x \int \frac{e^{2x}}{(e^x)^2} dx = e^x \int 1 dx = x e^x \\
y &= C_1 e^x + C_2 x e^x
\end{aligned}$$

**⑱ 題目：** 已知 $y_1=x$ 為解，求 $xy'' - y' = 0$ 之第二解

$$\begin{aligned}
y'' - \frac{1}{x}y' &= 0 \Rightarrow P(x) = -\frac{1}{x} \\
e^{-\int -\frac{1}{x} dx} &= e^{\ln x} = x \\
y_2 &= x \int \frac{x}{x^2} dx = x \int \frac{1}{x} dx = x \ln x \\
y &= C_1 x + C_2 x \ln x
\end{aligned}$$
