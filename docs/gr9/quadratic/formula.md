# the quadratic formula
*in this episode i set out on a quest to find out why the quadratic formula is so goofy*

## derivation
<div markdown class="md-has-sidebar">
<main markdown>
so basically the *idea* is you [complete the square](../complete) except with arbitrary coefficients in the quadratic equation $ax^2 + bx + c = 0$.

$$
ax^2 + bx = -c
$$
</main>
<aside markdown>
!!! note "$a\neq0$"
    it doesnt really matter because if you have $a=0$ just use linear equation stuff instead
</aside>
</div>

so now we need a number $n$ that we can add to both sides so that we can factorize the left side to $(x\sqrt{a}+n)^2$.

to do this we need it to "agree" with $b$ since we need $(x\sqrt{a})^2+2n(x\sqrt{a})+n^2$ on the left side which means

$$
\begin{aligned}
2n\sqrt{a} &= b \\
n &= \frac{b}{2\sqrt{a}}
\end{aligned}
$$

now we can do

$$
\begin{aligned}
ax^2 + bx + (\frac{b}{2\sqrt{a}})^2 &= -c + (\frac{b}{2\sqrt{a}})^2 \\
(x\sqrt{a})^2 + \cancel{2}(x\cancel{\sqrt{a}})(\frac{b}{\cancel{2}\cancel{\sqrt{a}}}) + (\frac{b}{2\sqrt{a}})^2 &= -c + \frac{b^2}{(2\sqrt{a})^2} \\
(x\sqrt{a} + \frac{b}{2\sqrt{a}})^2 &= \frac{-4ac + b^2}{(2\sqrt{a})^2} \\
x\sqrt{a} + \frac{b}{2\sqrt{a}} &= \pm\sqrt{\frac{b^2 - 4ac}{(2\sqrt{a})^2}} \\
&= \frac{\pm\sqrt{b^2 - 4ac}}{2\sqrt{a}} \\
x + \frac{b}{2a} &= \frac{\pm\sqrt{b^2 - 4ac}}{2a} \\
x &= \frac{-b\pm\sqrt{b^2 - 4ac}}{2a}
\end{aligned}
$$

oh hey, that formula looks familiar...

## cool shit you can do

### the funny discriminant thing
ok so like notice how we have $b^2-4ac$ in the square root so now if it's negative then we'll end up $i$ so we know from its sign whether the solution is real or complex *even if we don't know the coefficients themselves*, so $b^2-4ac$ is titled "THE discriminant" (like it's the only discriminant ever and cubic equations don't exist, just ignore those for now).

### root stuff
#### summing

so now you want to sum two roots but you're too lazy to actually do the math. what now?

$$
\begin{aligned}
x_1 &= \frac{-b+\sqrt{b^2 - 4ac}}{2a} \\
x_2 &= \frac{-b-\sqrt{b^2 - 4ac}}{2a}
\end{aligned}
\\
\begin{aligned}
x_1+x_2 &= \frac{-b+\sqrt{b^2 - 4ac}}{2a} + \frac{-b-\sqrt{b^2 - 4ac}}{2a} \\
&= \frac{-b\cancel{+\sqrt{b^2 - 4ac}}-b\cancel{-\sqrt{b^2 - 4ac}}}{2a} \\
&= \frac{-2b}{2a} \\
&= -\frac{b}{a} \\
\end{aligned}
$$

you're welcome.

#### multiplying
similarly,

$$
\begin{aligned}
x_1x_2 &= (\frac{-b + \sqrt{b^2 - 4ac}}{2a})(\frac{-b - \sqrt{b^2 - 4ac}}{2a}) \\
&= \frac{( (-b) + \sqrt{b^2 - 4ac} )( (-b)-\sqrt{b^2 - 4ac} )}{4a^2} \\
&= \frac{( \cancel{(-b)^2} - \cancel{b^2} - 4ac )}{4a^2} \\
&= -\frac{\cancel{4}\cancel{a}c}{\cancel{4}a\cancel{^2}} \\
&= -\frac{c}{a}
\end{aligned}
$$
