---
title: Mathematics Subject GRE refcard
author: Colton Grainger
revised: 2018-07-19
---

\newcommand{\RR}{\mathbf{R}}
\newcommand{\QQ}{\mathbf{Q}}
\newcommand{\NN}{\mathbf{N}}
\newcommand{\CC}{\mathbf{C}}
\newcommand{\eps}{\varepsilon}

> "As with any other ‘sport,’ basketball players need to stay in shape through regular ‘practice meets’," explains Gary Richardson, a "coach" of one of the camp’s teams. "You don’t want your bicep neurons to go weak."
>
> Ferguson, who started throwing a ball when he was only three years old, describes the camp in almost reverential terms. "At my high school," he says, "I was ostracized as a jock, teased and humiliated because I didn’t enjoy inverting matrices or grinding out Taylor series expansions. But here, I’ve finally found friends who share my passion for basketball."
>
> Don’t think, though, that life is all court and hoop for these precocious young wizards. Like anyone else, they need to unwind—except that when they do, their favored recreations are even odder than their eccentric passion. Rather than playing high-stakes Scrabble, beguiling one another with Goedelian logic puzzles, or composing poems without using the letter ‘e,’ these teens regale each other with anecdotes about beer and sex.

[Scott Aaronson, *[Trigonometry? No Way: These Teens Would Rather Toss a Ball](https://www.scottaaronson.com/writings/athletes.html)*]

These are question/answer pairs I used for rote memorization before the mathematics subject GRE. Here's the accompanying [tab separated text file](/2016-10-27-maths-GRE-flashcards.txt) for spaced repetition, e.g., mnemosyne. I used Steven A. Leduc's [Cracking the GRE Mathematics Subject Test](https://www.amazon.com/Cracking-GRE-Mathematics-Subject-Test/dp/0375429727).

Update (2019-05-27): The rest of this page is quite **outdated**. Consider perhaps looking at [these syllabi](https://www.cmi.ac.in//admissions/syllabus.php) from the Chennai Mathematical Institute.

## Functions

- Q: When is a function $f\colon A \to B$ said to be one-to-one? 
- A: Whenever no two elements in $A$ are mapped by $f$ to the same element in $B$. That is, $f$ is one-to-one if and only if $x_1 \neq x_2 \implies f(x_1) \neq f(x_2)$.
- Q: When is a function $f\colon A \to B$ said to be onto? 
- A: If every element in $B$ is the image of some element in $A$. That is, $f$ is onto if and only if for all $b \in B$, there exists $a \in A$ such that $f(a) = b$.
- Q: Suppose $f \colon A \to B$ is a function. When does the inverse function $f^{-1}\colon B \to A$ exist? Define it. 
- A: The proper inverse,$$f^{-1}\colon B \to A \text{ s.th. } f^{-1} \circ f = \text{id}_A \text{ and }f \circ f^{-1} = \text{id}_B,$$exists exactly when $f$ is both one-to-one and onto, i.e. when $f$ is a bijection. We define $f^{-1}:B \to A$ by $$f^{-1}(b) = a \Leftrightarrow f(a) = b.$$
- Q: Suppose $f \colon A \to B$ is a bijection. Define the inverse function $f^{-1} \colon B \to A$. 
- A: It is guaranteed that for every element $y$ in $B$ there is one, and only one, element $x$ in $A$ such that $f(x) = y$. So we define the inverse function $f^{-1} \colon B \to A$ by $$f^{-1}(y) = x \Leftrightarrow f(x) = y. $$
- Q: Define $f$ by the equation $f(x) = x^3 + x$. Given that this function has a well-defined inverse, determine the value of $f^{-1}(-2)$. 
- A: If $a = f^{-1}(-2)$, then by definition, $f(a) = -2$. So $$ f(a) = -2 \implies a^3 + a = -2. $$ By inspection, $a = -1$, so $f^{-1}(-2) = -1$.
- Q: Suppose $f \colon A \to B$ is a function. When does the ``left inverse" exist? 
- A: The left inverse, $$f^{\text{LI}}\colon B \to A \text{ s.th. } f^{\text{LI}} \circ f = \text{id}_B,$$ exists when $f$ is one-to-one.
- Q: Suppose $f \colon A \to B$ is a function.When does the ``right inverse" exist? 
- A: The right inverse, $$f^{\text{RI}} \colon B \to A \text{ s.th. } f \circ f^{\text{RI}} = \text{id}_B,$$ exists when $f$ is onto.

## Conic sections

- Q: What is the universal equation for conic sections?
- A: It is the second-degree equation in $x$ and $y$$$ Ax^2 + Bxy + Cy^2 + Dx + Ey + F = 0.$$
- Q: The equation for a straight line in the $xy$ plane is: 
- A: $$ax + by + c = 0$$ where $a$ and $b$ are both not zero.
- Q: Suppose a line in the $xy$ plane has a defined slope $m$ and passes through the point $(x_0,y_0)$. What is the equation of this line? 
- A: It is $y = m(x-x_0) + y_0$. This follows directly from the definition of slope$$ m = \frac{\Delta y}{\Delta x} = \frac{y - y_0}{x - x_0}. $$
- Q: When are two nonvertical lines in the plane perpendicular? 
- A: Exactly when the product of their slopes is $-1$.
- Q: Classically define a parabola and describe its features. 
- A: Let $F$ be a given fixed point and $D$ a given fixed line that doesn't contain $F$. A parabola is the set of points in the plane containing $F$ and $D$ that are equidistant from the point $F$ (the focus) and the line $D$ (the directrix). The axis of a parabola is the line through the focus and perpendicular to the directrix. The vertex of a parabola is the turning point, the point on the parabola's axis that is midway between the focus and the directrix.
- Q: What are the standard equations of the parabolas with vertices at the origin, foci at a distance $p$ from the origin, and axes either the $x$- or $y$- axis? 
- A: They are $$y = \pm \frac{1}{4p}x^2$$ and $$x = \pm \frac{1}{4p}y^2$$ with foci $(0,\pm p)$ and $(\pm p, 0)$ respectively.
- Q: What is the equation of a circle with radius $a$ centered at the origin? 
- A: It is $x^2 + y^2 = a^2$ or, equivalently, $$ \frac{x^2}{a^2} + \frac{y^2}{a^2} = 1.$$
- Q: What is equation of a circle with radius $a$ centered at the point $(h, k)$? 
- A: It is $$ \frac{(x-h)^2}{a^2} + \frac{(y-k)^2}{a^2} = 1.$$
- Q: Let $\mathbf{r}$ and $\mathbf{r}_0$ be vectors. What is the vector from $\mathbf{r}_0$ to $\mathbf{r}$? 
- A: It is $\mathbf{r} -\mathbf{r}_0$, i.e. ``to the point, from the source.''
- Q: Classically define an ellipse. 
- A: An ellipse is the set of points in the plane such that the sum of the distances from every point on the ellipse to two given fixed points (the foci) is a constant. (And to avoid a degenerate case, the constant sum must be greater than the distance between the foci.)
- Q: Describe the features of an ellipse. 
- A: The longer symmetry axis of an ellipse is called the major axis (on which the foci are located), the shorter one is the minor axis. The endpoints of the major axis are the vertices. The eccentricity of an ellipse is the ratio of the length of the segment connecting the foci to the length of the minor axis.
- Q: What is the standard equation of an ellipse centered at the origin---with axes parallel to the coordinate axes? 
- A: It is $$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1. $$
- Q: Consider the real numbers $a$ and $b$ with $a > b > 0$. Suppose we have an ellipse with equation$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1. $$ Where are the vertices? What is the length of the major axis? Where are the foci? What is the eccentricity? 
- A: FLAT PANCAKE. The vertices are at $(\pm a, 0)$. The major axis has length $2a$. With $c = \sqrt{a^2 - b^2}$, the foci are at $(\pm c, 0)$. The eccentricity is $e = c/a$.
- Q: Consider the real numbers $a$ and $b$ with $b > a > 0$. Suppose we have an ellipse with equation$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1. $$ Where are the vertices? What is the length of the major axis? Where are the foci? What is the eccentricity? 
- A: TALL PANCAKE. The vertices are at $(0, \pm b)$. The major axis has length $2b$. With $c = \sqrt{b^2 - a^2}$, the foci are at $(0, \pm c)$. The eccentricity is $e = c/b$.
- Q: Classically define a hyperbola. 
- A: A hyperbola is the set of points in the plane such that the difference between the distances from every point on the hyperbola to two fixed points (the foci) is a constant. (And to avoid a degenerate case, the constant difference must be smaller than the distance between the foci.)
- Q: Describe the features of a hyperbola (branches, asymptotes, focal axis, center). 
- A: A hyperbola consists of two seperate curves called branches. These branches are seperated by two asymptotes. The foci are situated in the regions of positive concavity. The line that contains the foci is called the focal axis; the midpoint of the segment joining the foci is the center or the hyperbola.
- Q: What is the standard equation of a hyperbola centered at the origin with the $x$-axis as the focal axis? Does this hyperbola intersect the $y$-axis? 
- A: It is $$\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1.$$ Because there exists no real $y$ such that$$0-\frac{y^2}{b^2} = 1,$$ we know this hyperbola does not intersect the $y$-axis.
- Q: What is the standard equation of a hyperbola centered at the origin with the $y$-axis as the focal axis? Does this hyperbola intersect the $x$-axis? 
- A: It is $$\frac{y^2}{b^2} - \frac{x^2}{a^2} = 1.$$ Because there exists no real $x$ such that$$0-\frac{x^2}{a^2} = 1,$$ we know this hyperbola does not intersect the $x$-axis.
- Q: Consider the hyperbola with equation $$\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1.$$Where are the foci? Where are the vertices? 
- A: With $c = \sqrt{a^2 + b^2}$, the foci are at $(\pm c, 0)$. The vertices are at $(\pm a, 0)$.
- Q: Consider the hyperbola with equation $$\frac{y^2}{b^2} - \frac{x^2}{a^2} = 1.$$Where are the foci? Where are the vertices? 
- A: With $c = \sqrt{a^2 + b^2}$, the foci are at $(0,\pm c)$. The vertices are at $(0, \pm b)$.

## Polynomial manipulation

- Q: Let $p(x)$ and $d(x)$ be polynomials with the degree of $d(x)$ less than or equal to the degree of $p(x)$. If $d(x)$ is not identically zero, the division algorithm guarantees what? 
- A: The division algorithm guarantees that dividing $p(x)$ by $d(x)$ gives unique polynomials $q(x)$ and $r(x)$ such that $$ p(x) = q(x)d(x) + r(x)$$ where either $r(x)$ is identically zero or the degree of $r(x)$ is less than the degree of $d(x)$. The polynomial $q(x)$ is known as the quotient; the polynomial $r(x)$ is known as the remainder.
- Q: Let $p(x)$ be a polynomial of degree at least 1 and define another degree 1 polynomial $d(x) = x - k$ (where $k$ is a complex number). If $p(x)$ is divided by $d(x)$, there exist unique polynomials $q(x)$ and $r(x)$ such that $$ p(x) = q(x) \cdot (x-k) + r$$where $r$ is a constant. State the Remainder Theorem. 
- A: Substituting $x = k$ into the equation yields $p(k) = r$. Therefore, when $p(x)$ is divided by $x-k$, the remainder is $p(k)$.
- Q: Let $p(x)$ be a polynomial of degree at least 1. The remainder theorem states ``when $p(x)$ is divided by $x-k$, the remainder is $p(k)$.'' From these grounds, state and prove the Factor Theorem. 
- A: 
    - The Factor Theorem states that $x=k$ is a root of the polynomial equation $p(x) = 0$ if and only if $x-k$ is a factor of $p(x)$.
    - Suppose $x=k$ satisfies $p(x) = 0$. Then $p(k) = 0$. The Remainder theorem states $$ p(x) = q(x) \cdot (x-k) + p(k)$$ and substitution implies$$p(x) =q(x) \cdot (x-k) + 0.$$ So $x-k$ is a factor of $p(x)$. Conversely, suppose$x-k$ is a factor of $p(x)$. Then$$p(x) =q(x) \cdot (x-k).$$ I claim $x=k$ satisfies $p(x) = 0$. Well, $p(x) = 0$ exactly when $$q(x) \cdot (x-k)= 0.$$ This is true when $x =k$.
- Q: State the Fundamental Theorem of Algebra. 
- A: Every polynomial equation $$a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x+a_0 = 0$$ of degree $n \geq 1$ has at least one (real or complex) root.
- Q: How can the polynomial $$a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x+a_0$$ be written as the product of unique, linear (degree 1) factors? 
- A: We find that $$a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x+a_0 = a_n(x-k_1)(x-k_2)\cdots(x-k_n)$$ using the division algorithm repeatedly.
- Q: If the coefficients of$$p(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x+a_0$$ are integers, then the Rational Roots Theorem states 
- A: if the equation $p(x) = 0$ has any rational roots, then, when expressed in lowest terms, they must be of the form $$x = \frac{s}{t}$$ where $s$ is a factor (positive or negative) of the constant term $a_0$ and $t$ is a factor(positive or negative)of the leading coefficient $a_n$.
- Q: If the coefficients of$$p(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x+a_0$$ are rational, then the Conjugate Roots Theorem states 
- A: if the equation $p(x) = 0$ has a root of the form $x = s +t\sqrt{u}$ (where where $s$ and $t$ are rational and $\sqrt{u}$ is irrational), then the equation must also have the conjugate radical, $x = s - t\sqrt{u}$, as a root.
- Q: If the coefficients of$$p(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x+a_0$$ are real, then the Complex Conjugate Roots Theorem states 
- A: if the equation $p(x) = 0$ has a root of the form $x = s +ti$ (where $s$ and $t$ are real numbers and $i^2 =-1$), then the equation must also have the complex conjugate, $x = s - ti$, as a root.
- Q: Consider the polynomial equation $$p(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x+a_0$$ where $a_n \neq 0$. What is the sum of the $n$ roots? What is the product of the $n$ roots? 
- A: The sum of the roots is $$\frac{-a_{n-1}}{a_n}.$$ The product of the roots is $$(-1)^n\frac{a_0}{a_n}.$$ If the polynomial is monic, then the sum of the roots is $-a_{n-1}$ and the product of the roots is $(-1)^na_0$.
- Q: Factor $x^4+1$. 
- A: We find\begin{align*}x^4+1 &= x^4+2x^2+1-2x^2,\\&= (x^2+1)^2-(\sqrt{2}x)^2,\\&= (x^2+1 - \sqrt{2}x)(x^2+1+\sqrt{2}x),\\&=(x^2 - \sqrt{2}x+1)(x^2+\sqrt{2}x+1).\end{align*}

## Exponential functions and logarithms

- Q: Logarithms are exponents. Whence $\log_bx = y$ means 
- A: $b^y = x$.
- Q: The function $f^{-1}(y) = \log_by$ is the inverse of the exponential function $f(x)= b^x$. State the domain of the identity function $$(f^{-1} \circ f)(x) = \log_b(b^x)$$ and the domain of the other identity function $$(f \circ f^{-1})(y) =b^{\log_b(y)}.$$ 
- A: The domain of $f^{-1} \circ f$ is $\mathbf{R}$. The domain of $f \circ f^{-1}$ is $\{y \in \mathbf{R} : y > 0\}$.
- Q: What restrictions exist on $b$ such that $x = \log_b(y)$ is the well defined inverse function of $y = b^x$? 
- A: We require $b > 0$ and $b \neq 1$.
- Q: Suppose $0 < b < 1$. Is $f(x) = \log_b(x)$ increasing or decreasing? 
- A: If $0 < b < 1$, then$f(x) = \log_b(x)$is decreasing.
- Q: Simplify$\log_b(x_1x_2)$. 
- A: Let $y_1 = \log_b(x_1)$ and $y_2 = \log_b(x_2)$. Then $$b^{y_1} = x_1 \text{ and } b^{y_2} = x_2.$$ Taking the product,$$ x_1x_2 =b^{y_1}b^{y_2} = b^{y_1 + y_2}.$$Whence $$\log_b(x_1x_2) = y_1 + y_2 = \log_b(x_1)+\log_b(x_2).$$
- Q: Simplify$\log_b(x^a)$. 
- A: Let $\log_b(x) = y$. Then $b^y = x$. So $$x^a = (b^y)^a = b^{ya} = b^{ay}.$$ Because logarithms are exponents, $$x^a =b^{ay} \implies \log_b(x^a) = ay.$$ Substituting $y= \log_b(x)$, $$\log_b(x^a) = a\log_b(x).$$
- Q: For what value of $k$ is $$k\log_a(x) = \log_b(x)?$$ 
- A: For $k = \log_b(a)$, we find $$\log_b(a)\log_a(x) = \log_b(x).$$ This is an identity, proven as follows:Let $y_1 =\log_b(a)$ and $y_2 =log_a(x)$. Then $$b^{y_1} = a \text{ and } a^{y_2} = x.$$ Substitution of $b^{y_1}$ for $a$ yields $$x = (b^{y_1})^{y_2} = b^{y_1y_2}.$$Because logarithms are exponents, $y_1y_2 = \log_b(x)$. Thus $$\log_b(a)\log_a(x) = \log_b(x).$$
- Q: Let $a>0$. Express this function ($f\colon \RR^+ \to \RR$) in terms of natural logarithms:$$f(x) = \log_a(x).$$ 
- A: For $a,b>0$ It can be proven that $$\log_b(a)\log_a(x) = \log_b(x).$$Setting $b = e$ and dividing by $\ln(a)$we find $$\log_a(x) = \frac{\ln(x)}{\ln(a)}.$$

## Matrix algebra

These questions are from [Paul Hand](http://www.leadinglesson.com/), included here under fair use.

- Q: Let $\mathbf{A}$ be an $n \times n$ matrix. Linear equations of the form $\mathbf{A}\mathbf{x}=\mathbf{b}$ are called inhomogeneous if $\mathbf{b}\neq 0$.If $\text{det} \mathbf{A}\neq 0$ 
- A: then $\mathbf{A}\mathbf{x}=\mathbf{b}$ has exactly one solution, $\mathbf{x}=\mathbf{A}^{-1}\mathbf{b}$.
- Q: Let $\mathbf{A}$ be an $n \times n$ matrix. Linear equations of the form $\mathbf{A}\mathbf{x}=\mathbf{b}$ are called inhomogeneous if $\mathbf{b}\neq 0$. If $\text{det}\mathbf{A}=0$ 
- A: then $\mathbf{A}\mathbf{x}=\mathbf{b}$ has either no solutions or infinitely many solutions.
- Q: If $\mathbf{A}$ is square and invertible, what is the solution to $\mathbf{A}\mathbf{x} = \mathbf{b}$? 
- A: The solution is $\mathbf{x} = \mathbf{A}^{-1}\mathbf{b}$.
- Q: What is the inverse of the $2 \times 2$ matrix$\left(\begin{array}{cc}a & b \\c & d \\\end{array}\right)$? 
- A: The inverse of a $2 \times 2$ matrix is given by swapping the diagonal entries, negating the off-diagonal entries, and dividing by the determinant:$$\left(\begin{array}{cc}a &b \\c & d \\\end{array}\right)^{-1} = \frac{1}{ad-bc}\left(\begin{array}{cc}d & -b \\-c & a \\\end{array}\right).$$ The inverse is not defined if the determinant is zero.
- Q: What is the inverse of the $3 \times 3$ matrix$\left(\begin{array}{ccc}a &b & c\\d & e &f \\g &h &i\end{array}\right)$? 
- A: To find the inverse of a $3 \times 3$ matrix,
    - Compute the minors of each element;
    - Negate every other element, according to a checkerboard pattern;
    - Take the transpose;
    - Divide by the determinant of the original matrix.
  The inverse is not defined if the determinant is zero. Note:the minor of the $(i,j)$th entry of a matrix $\mathbf{A}$ is the determinant of the submatrix obtained by removing the $i$th row and the $j$th column of $\mathbf{A}$.

## Vector geometry

- Q: What is the equation of a line in $\mathbf{R}^2$ with normal vector $\mathbf{n}$? 
- A: The line is given by $$\mathbf{n}\cdot\mathbf{x} = b$$ for some fixed real value $b$.
- Q: Write the equation of a line in $\mathbf{R}^2$ which intersects a point $\mathbf{x}_0$ and has the normal vector $\mathbf{n}$. 
- A: The line in $\mathbf{R}^2$ going through $\mathbf{x}_0$ with normal vector $\mathbf{n}$ is given by$$\mathbf{n}\cdot\mathbf{x} = \mathbf{n}\cdot\mathbf{x}_0.$$
- Q: State three ways to find a vector perpendicular to $\mathbf{x}$. 
- A: 
    - In $\mathbf{R}^2$ a vector perpendicular to $\mathbf{x} = \langle a, b \rangle$ is $\langle -b,a \rangle$.
    - Write and solve the equation $\mathbf{x} \cdot \mathbf{y} = 0$.
    - Take the cross product with any vector that is not a multiple of $\mathbf{x}$.

## Trigonometry

- Q: Consider a ray, with initial point at the origin, rotated in the plane to form an angle, $\theta$, with the positive $x$-axis as its initial side. Choose any point $P:(x,y)$ in the plane---except for the origin---on the ray and let $r$ be the distance to $P$ from the origin. What is $\sin\theta$? 
- A: $\sin\theta = \frac{y}{r}.$
- Q: Consider a ray, with initial point at the origin, rotated in the plane to form an angle, $\theta$, with the positive $x$-axis as its initial side. Choose any point $P:(x,y)$ in the plane---except for the origin---on the ray and let $r$ be the distance to $P$ from the origin. What is $\cos\theta$? 
- A: $\cos\theta = \frac{x}{r}.$
- Q: Consider a ray, with initial point at the origin, rotated in the plane to form an angle, $\theta$, with the positive $x$-axis as its initial side. Choose any point $P:(x,y)$ in the plane---except for the origin---on the ray and let $r$ be the distance to $P$ from the origin. What is $\tan\theta$? 
- A: $\tan\theta = \frac{y}{x}.$
- Q: Consider a ray, with initial point at the origin, rotated in the plane to form an angle, $\theta$, with the positive $x$-axis as its initial side. Choose any point $P:(x,y)$ in the plane---except for the origin---on the ray and let $r$ be the distance to $P$ from the origin. What is $\sec\theta$? 
- A: $\sec\theta = \frac{r}{x}.$
- Q: Consider a ray, with initial point at the origin, rotated in the plane to form an angle, $\theta$, with the positive $x$-axis as its initial side. Choose any point $P:(x,y)$ in the plane---except for the origin---on the ray and let $r$ be the distance to $P$ from the origin. What is $\csc\theta$? 
- A: $\csc\theta = \frac{r}{y}.$
- Q: Consider a ray, with initial point at the origin, rotated in the plane to form an angle, $\theta$, with the positive $x$-axis as its initial side. Choose any point $P:(x,y)$ in the plane---except for the origin---on the ray and let $r$ be the distance to $P$ from the origin. What is $\cot\theta$? 
- A: $\cot\theta = \frac{x}{y}.$
- Q: Express $\tan\theta$, $\csc\theta$ and $\sec\theta$ in terms of sine and cosine. 
- A: By definition\begin{align}\tan\theta &= \frac{\sin\theta}{\cos\theta},\\\csc\theta &= \frac{1}{\sin\theta},\\\sec\theta &= \frac{1}{\cos\theta}.\end{align}
- Q: Express $\cot\theta$ in terms of $\tan\theta$. 
- A: By definition $\cot\theta = \frac{1}{\tan\theta}$.
- Q: State the opposite angle identities. 
- A: It can be seen that sine as an odd function$$ \sin(-\theta) = -\sin\theta $$ and cosine is an even function $$\cos(-\theta) = \cos\theta.$$
- Q: From $\sin^2\theta + \cos^2\theta = 1$ derive the other two pythagorean identities. 
- A: Divide by $\sin^2\theta$ to find$$\frac{\sin^2\theta}{\sin^2\theta} + \frac{\cos^2\theta}{\sin^2\theta} = \frac{1}{\sin^2\theta}\implies 1 + \cot^2\theta = \csc^2\theta.$$Divide by $\cos^2\theta$ to find$$\frac{\sin^2\theta}{\cos^2\theta} + \frac{\cos^2\theta}{\cos^2\theta} = \frac{1}{\cos^2\theta}\implies \tan^2\theta + 1 = \sec^2\theta.$$
- Q: Derive the addition formulas for $\sin(\alpha + \beta)$ and $\cos(\alpha + \beta)$. 
- A: Write the complex number $$\cos(\alpha + \beta) + i\sin(\alpha + \beta).$$ By definition of the complex exponential function,\begin{align*}&\cos(\alpha + \beta) + i\sin(\alpha + \beta)\\&= e^{i(\alpha+\beta)}\\&=e^{i\alpha} e^{i\beta}\\&=(\cos\alpha + i\sin\alpha)(\cos\beta+i\sin\beta)\\&=\cos\alpha\cos\beta + i\cos\alpha\sin\beta +i\sin\alpha\cos\beta -\sin\alpha\sin\beta\\&= (\cos\alpha\cos\beta - \sin\alpha\sin\beta) + i(\cos\alpha\sin\beta+\sin\alpha\cos\beta).\end{align*}Equate the real and imaginary parts.
- Q: Derive the addition formula for $\tan(\alpha + \beta)$. 
- A: \begin{align*}\tan(\alpha + \beta) &= \frac{\sin(\alpha + \beta)}{\cos(\alpha + \beta)}\\&= \frac{\cos\alpha\sin\beta+\sin\alpha\cos\beta}{\cos\alpha\cos\beta - \sin\alpha\sin\beta}\\&=\frac{\frac{\sin\beta}{\cos\beta}+\frac{\sin\alpha}{\cos\alpha}}{1 - \frac{\sin\alpha\sin\beta}{\cos\alpha\cos\beta}}\\&= \frac{\tan\beta + \tan\alpha}{1 - \tan\alpha\tan\beta}\end{align*}
- Q: Derive the subtraction formula for $\tan(\alpha - \beta)$. 
- A: \begin{align*}\tan(\alpha - \beta) &= \frac{\sin(\alpha - \beta)}{\cos(\alpha - \beta)}\\&= \frac{-\cos\alpha\sin\beta+\sin\alpha\cos\beta}{\cos\alpha\cos\beta + \sin\alpha\sin\beta}\\&=\frac{-\frac{\sin\beta}{\cos\beta}+\frac{\sin\alpha}{\cos\alpha}}{1 + \frac{\sin\alpha\sin\beta}{\cos\alpha\cos\beta}}\\&= \frac{-\tan\beta + \tan\alpha}{1 + \tan\alpha\tan\beta}\end{align*}
- Q: Write the addition formulas for $\cos(\alpha + \beta)$ and $\sin(\alpha + \beta)$. Then derive the formulas for $\cos(\alpha - \beta)$ and $\sin(\alpha - \beta)$. 
- A: Consider real and imaginary parts\begin{align*}&\cos(\alpha + \beta) + i\sin(\alpha + \beta) \\& = \left[\cos\alpha\cos\beta - \sin\alpha\sin\beta\right] + i\left[\cos\alpha\sin\beta+\sin\alpha\cos\beta\right].\end{align*}Recalling $\cos(-\beta) = \cos\beta$ and $\sin(-\beta) = -\sin\beta$,\begin{align*}&\cos(\alpha + (-\beta)) + i\sin(\alpha +(-\beta)) \\& = \left[\cos\alpha\cos(-\beta) - \sin\alpha\sin(-\beta)\right] + i\left[\cos\alpha\sin(-\beta)+\sin\alpha\cos(-\beta)\right]\\& = \left[\cos\alpha\cos\beta + \sin\alpha\sin\beta\right] + i\left[-\cos\alpha\sin\beta+\sin\alpha\cos\beta\right].\end{align*}
- Q: In the (polar coordinate) plane, what is the equation of a circle with the line segment from the origin to the point $(2a, 0)$ as a diameter (for any nonzero $a \in \RR$)? 
- A: Intuitively picturing the cosine function ``rolled around" the origin, we find$$r(\theta) = 2a\cos(\theta)$$ where $r$ is a function of $\theta$. If $a>0$, then the circle lies on the $\theta = 0$ side of the origin. If $a <0$, then the circles lies on the $\theta = \pi$ side of the origin.
- Q: In the plane, what is the polar equation of a circle with diameter connecting the origin to the point $(2a, 0)$? 
- A: Picturing the cosine function ``rolled around" the origin, we find$$r(\theta) = 2a\cos(\theta)$$ where $r$ is a function of $\theta$.
    - If $a>0$, the circle lies in the $\theta = 0$ direction.
    - If $a <0$, the circles lies in the $\theta = \pi$ direction.
- Q: In the plane, what is the polar equation of a circle with diameter connecting the origin to the point $(2a, \frac{\pi}{2})$? 
- A: Picturing the sine function ``rolled around" the origin, we find$$r(\theta) = 2a\sin(\theta)$$ where $r$ is a function of $\theta$.
    - If $a>0$, the circle lies in the $\theta = \frac{\pi}{2}$ direction.
    - If $a <0$, the circles lies in the $\theta = -\frac{\pi}{2}$ direction.
- Q: In the plane, what is the polar equation of a cardioid with axis of symmetry connecting the origin to the point a radial distance of $4a$ away at an angle of $\theta =0$? 
- A: Picturing a upshifted cosine function ``rolled around" the origin, we find$$r(\theta) = 2a(1+\cos(\theta))$$ where $r$ is a function of $\theta$. Note that $a>0$ implies the cardioid lies in the $\theta = 0$ direction.
- Q: Express $\sin 2\theta$ in terms of $\cos\theta$ and $\sin\theta$. 
- A: Given $$\sin(\alpha+\beta) = \cos\alpha\sin\beta + \sin\alpha\cos\beta,$$ substitute $\theta = \alpha = \beta$ to find $$\sin(2\theta) = 2\sin\theta\cos\theta.$$
- Q: Express $\cos 2\theta$ in terms of $\cos\theta$ and $\sin\theta$. 
- A: Given $$\cos(\alpha+\beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta,$$ substitute $\theta = \alpha = \beta$ to find $$\cos(2\theta) = \cos^2\theta - \sin^2\theta.$$ By Pythagorean identity, we may also find$$\cos(2\theta) = 1 - 2\sin^2\theta = 2\cos^2\theta - 1.$$
- Q: Express $\tan 2\theta$ in terms of $\tan\theta$. 
- A: From $$\tan(\alpha + \beta)= \frac{\tan\beta + \tan\alpha}{1 - \tan\alpha\tan\beta}$$ we let $\theta = \alpha = \beta$ to find $$\tan 2\theta =\frac{2\tan\theta}{1 - \tan^2\theta}.$$

## Sequences and series

- Q: We say that a sequence, $\{x_n\}\subseteq \RR$, converges to $L$, or that $L$ is the limit of the sequence, written as $x_n \to L$, if and only if (give the distance metric definition) 
- A: for every $\eps >0$ there exists a natural number, $N$, such that the distance to $x_n$ from $L$ is less than $\eps$ for every natural number $n > N$.
- Q: If $\{x_n\} \subseteq \RR$ is a sequence, then we say that $x_n$ converges to $L$, or that $L$ is the limit of the sequence, if and only if (give the topological definition) 
- A: for every $\RR_{std}$-open set $U$ containing $L$, there is an $N \in \NN$ such that $x_n \in U$ for all $n > N$.
- Q: Let $\{x_n\} \subseteq \RR$ be a sequence. Suppose that there does not exist $L$ such that for any $\eps > 0$ there is an $N \in \mathbf{N}$ such that $n > N$ implies $|x_n - L| < \eps$. We say? We write? 
- A: We say the sequence is divergent---it diverges. We write $$\lim x_n \text{D.N.E.}.$$
- Q: A sequence $\{x_n\} \subseteq \RR$ is said to be monotonic iff 
- A: it is eventually increasing $$(x_n \leq x_{n+1} \text{ for every }n > N \text{ for some }N \in \NN)$$ or eventually decreasing $$(x_n \geq x_{n+1} \text{ for every }n > N \text{ for some }N \in \NN).$$
- Q: Define a bounded sequence. Then describe the relation between boundedness and convergence. 
- A: A sequence $\{x_n\}$ is bounded if and only if there exists a real $M > 0$ such that $|x_n| \leq M$ for all $n \in \NN$. If a sequence is convergent, then it is bounded.
- Q: State the Monotonic Convergence Theorem. 
- A: If a sequence $(x_n)$ is monotonic and bounded,then $(x_n)$ is convergent.
- Q: If $k$ is a constant, and $(a_n)$ converges to $A$, 
- A: then $(ka_n) \to kA$.
- Q: If $(a_n)$ converges to $A$ and $(b_n)$ converges to $B$, what is the limit of the sum, the difference, the product, and the quotient of $(a_n)$ and $(b_n)$? 
- A: \begin{align*}(a_n + b_n) &\to A + B;\\(a_n - b_n) &\to A - B;\\(a_nb_n) &\to AB;\\\left(\frac{a_n}{b_n}\right) &\to \frac{A}{B} \text{ (with } B \neq 0).\end{align*}
- Q: Let $k > 0$ be a constant and consider the sequence $\left\{\frac{1}{n^k}\right\}_{n \in \NN}$. What is $\text{lim }\frac{1}{n^k}?$ 
- A: With $k>0$, we have $\frac{1}{n^k} \to 0.$
- Q: Let $|k| > 1$ be a constant and consider the sequence $\left\{\frac{1}{k^n}\right\}_{n \in \NN}$. What is $$\lim_{n\to\infty}\frac{1}{k^n}?$$ 
- A: First write $$\frac{1}{k^n} = \left(\frac{1}{k}\right)^n.$$ With $|k| > 1$, we have $\left|\frac{1}{k}\right| < 1$. It can be proven that $$\lim_{n\to\infty} \left(\frac{1}{k}\right)^n = 0.$$
- Q: State the Squeeze Theorem. 
- A: Assume that $(a_n)$ and $(c_n)$ are sequences that converge to the same limit $L$. If $(b_n)$ is a sequence such that $$a_n \leq b_n \leq c_n$$ for every $n >N$ (for some $N \in \NN$), then $$(b_n) \to L.$$
- Q: Let $D \subseteq \NN$ be a set and $(a_n)$ be a sequence. Consider a function $f\colon D \to \CC$ such that $a_n = f(n)$ for all $n \in \NN$. What is $$\lim a_n?$$ 
- A: It can be shown that$$\lim a_n = L \Leftrightarrow \lim_{x \to \infty} f(x) = L.$$ Note: $\lim_{x \to \infty} f(x)$ may be found using L'H\^opital's rule.
- Q: Consider a sequence $\{x_n\}_{n\in\NN}$ and a natural number $N$. Define another sequence $\{\alpha_n\}_{n\in\NN}$ by $$\alpha_n = x_{n+N} \text{ (for all } n \in \NN).$$ What is the relationship (regarding convergence) between $\{x_n\}$ and $\{\alpha_n\}$? 
- A: I postulate that\begin{align*}\{x_n\} \text{ converges } &\Leftrightarrow \{\alpha_n\} \text{ converges;}\\x_n \to L &\Leftrightarrow \alpha_n \to L.\end{align*}
- Q: Consider the sequence $\{a_n\}_{n\in\NN}$ and the series $\sum_{n=1}^{\infty}a_n$. If the series $$\sum_{n=1}^{\infty}a_n$$ converges, what is the limit of the sequence $$\{a_n\}_{n\in\NN}?$$ 
- A: If $\sum a_n$ coverges, then $a_n \to 0$.
- Q: Let $k$ be a constant and suppose $\sum_{n=1}^{\infty}a_n$ converges. What value does $\sum_{n=1}^{\infty}ka_n$ coverge to? 
- A: We find $$\sum_{n=1}^{\infty}ka_n = k\sum_{n=1}^{\infty}a_n.$$
- Q: Let $k$ be a constant and suppose $\sum_{n=1}^{\infty}a_n$ diverges. Does $\sum_{n=1}^{\infty}ka_n$ diverge too? 
- A: Yes; if $k$ is a nonzero constant, then $$\sum_{n=1}^{\infty}ka_n$$ diverges. Of course, if $k=0$, the series converges to $0$.
- Q: If both $\sum_{n=1}^{\infty}a_n$ and $\sum_{n=1}^{\infty}b_n$ converge, does $$\sum_{n=1}^{\infty}(a_n+b_n)$$ converge? If so, what value does this series converge to? 
- A: If both $\sum_{n=1}^{\infty}a_n$ and $\sum_{n=1}^{\infty}b_n$ converge, then $$\sum_{n=1}^{\infty}(a_n+b_n)$$ converges as well. We may prove that $$\sum_{n=1}^{\infty}(a_n+b_n) = \sum_{n=1}^{\infty}a_n+\sum_{n=1}^{\infty}b_n.$$
- Q: Assume that $0 \leq a_n \leq b_n$ for all $n > N$. What is the convergence relationship between $\sum_{n=1}^{\infty}a_n$ and $\sum_{n=1}^{\infty}b_n$? 
- A: \begin{align*}\sum_{n=1}^{\infty}b_n \text{ covn. } &\implies \sum_{n=1}^{\infty}a_n\text{ covn. }\\\sum_{n=1}^{\infty}a_n \text{ div. } &\implies\sum_{n=1}^{\infty}b_n\text{ div. }\end{align*}
- Q: Consider a series $\sum_{n=1}^{\infty}a_n$. State the integral test for convergence. 
- A: If $f(x)$ is a positive, monotonically decreasing function for $x\geq 1$, such that $f(n) = a_n$ for all $n$ in $\NN$, then $$\sum_{n=1}^{\infty}a_n \text{ conv. } \Leftrightarrow \int_1^\infty f(x)dx \text{ conv.}$$
- Q: Consider a series $\sum_{n=1}^{\infty}a_n$. State the geometric series test for convergence. 
- A: A series, $\sum_{n=1}^{\infty}a_n$, is called geometric if and only if $$a_n = kr^n$$ for some constant $k$. The limit of a geometric series is, pneumatically, $$\frac{\text{first term}}{1-\text{ ratio between terms}}.$$
- Q: State the p-series test for convergence. 
- A: The series $$\sum_{n=1}^\infty \frac{1}{n^p}$$ converges if and only if $p>1$; $\sum1/{n^p}$ diverges when $p \leq 1$. When $p = 1$, the (harmonic) series $\sum 1/n$ diverges.
- Q: Consider a series $\sum_{n=1}^{\infty}a_n$. State the ratio test for absolute convergence. 
- A: We'll test $\sum a_n$ for absolute convergence. Form the limit $$L = \lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|.$$ Then,\begin{align*}&L < 1 \implies \sum |a_n| \text{ conv }\\&L > 1\implies \sum |a_n| \text{ div }\\&L = 0 \text{ the test is inconclusive}).\end{align*}
- Q: Consider a series $\sum_{n=1}^{\infty}a_n$ of nonnegative terms $a_n$. State the root test for convergence. 
- A: Form the limit $$L = \lim_{n\to\infty}\sqrt[n]{a_n}.$$ Then,\begin{align*}L < 1 &\implies \sum a_n \text{ conv }\\L > 1 &\implies \sum a_n \text{ div }\\(\text{when }L = 0 \text{ the test is inconclusive}).\end{align*}
- Q: Define an alternating series. 
- A: Suppose $\{a_n\}$ is a sequence of nonnegative real numbers. Then we call $$\sum_{n=1}^{\infty}(-1)^{n+1}a_n$$ an alternating series.
- Q: Suppose $\{a_n\}$ is a sequence of nonnegative real numbers and consider $$\sum_{n=1}^{\infty}(-1)^{n+1}a_n.$$ State the alternating series test. 
- A: The alternating series $\sum_{n=1}^{\infty}(-1)^{n+1}a_n$ will converge provided the terms $a_n$ decrease monotonically with a limit of zero.
- Q: Define absolute convergence. 
- A: Given a series $\sum a_n$ with real (not necessarily positive) terms, we can form the series $\sum |a_n|$ all of whose terms are clearly nonnegative. $$\text{If } \sum |a_n| \text{ converges, then } \sum a_n \text{ converges absolutely.}$$ Here's a fact: every absolutely convergent series converges.
- Q: Define conditional convergence. 
- A: Given a series $\sum a_n$ with real (not necessarily positive) terms, we can form the series $\sum |a_n|$ all of whose terms are clearly nonnegative. If $\sum |a_n|$ diverges yet $\sum a_n$ converges, then $\sum a_n$ converges conditionally (i.e., based on the order of terms added).

## Continuity 

- Q: A real number $x$ is a limit point of the set $A\subseteq\RR$ if and only if 
- A: either
    - $x = \lim{a_n}$ for some sequence of real numbers $\{a_n\}_{n\in\NN}$ contained in a set $A$ satisfying $a_n \neq x$ for all $n \in \NN$; or
    - for every $\RR_{std}$-open set $U$ containing $x$, the intersection $(U\setminus\{x\})\cap A$ is not empty.
- Q: A function $f\colon D \subseteq \RR \to \RR$ is continuous at a point $x$ if and only if (state the distance metric definition) 
- A: for every $\eps>0$ there is a $\delta >0$ such that $$\text{if } z\in D \text{ and } |x-z|<\delta \text{ then } |f(x)-f(z)|<\eps.$$ We say that $f$ is continuous if it is continuous at every point $x$ in its domain $D$.
- Q: A function $f\colon D \subseteq \RR \to \RR$ is continuous $x$ if and only if (state the topological definition) 
- A: for every $\RR_{std}$-open set $U \subseteq \RR$, $f^{-1}(U)$ is open in $D$ (where $D$ is given the subspace topology from $\RR_{std}$).
- Q: Consider the function $f\colon D \subseteq \RR \to \RR$. The limit of the function $f(x)$ (as $x$ approaches $a$) is $L$ if and only if 
- A: either 
    - for every sequence $(x_n) \subseteq D$ such that $x_n \to a$, the sequence $(f(x_n))$ converges to $L$; or
    - for every $\eps>0$ there is a $\delta >0$ such that $$\text{if } x\in D \text{ and } |x-a|<\delta \text{ then } |f(x)-L|<\eps.$$
  In either case we write $\lim_{x\to a} f(x) = L$.

- Q: We say that a function $f$ is continuous at $a$ if and only if (point-limit definition)
- A: it is true that $$\lim_{x\to a} f(x) = f(a).$$First, $f$ must be defined at $x =a$ (so that $f(a)$ exists); second, the limit of $f(x)$ as $x \to a$ must exist (and be finite); and third, this limit must be equal to the value of $f$ at $x=a$.
- Q: For what values of $x \in \RR$ are the following functions cts? 
    - Any constant function, $f(x) =k$
    - Any polynomial function, $$f(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x + a_0$$
    - Any exponential function, $f(x) = k^x$ (with $k>0$)
- A: Everywhere! That is, for all values $x$ in $\RR$.
- Q: The following functions are continuous everywhere they're defined: 
- A: 
    - Every function of the form $f(x) = x^r$ (with $r \in \QQ$)
    - The logarithm function, $f(x) = \log x$
    - The trig functions
- Q: If the functions $f$ and $g$ are both continuous at $a$, then each of the following functions is also continuous at $a$: 
- A: 
    - $(f+g)(x) = f(x)+g(x)$
    - $(f\cdot g)(x) =f(x)\cdot g(x)$
    - $\left(\frac{f}{g}\right)(x) = \frac{f(x)}{g(x)}$ (provided that $g(a) \neq 0$)
- Q: If $f:X \to Y$ is continuous at $a \in X$ and $g:Y \to Z$ is continuous at $f(a) \in Y$, is the composite function $g \circ f : X \to Z$ continuous at $x =a$? 
- A: Of course it is!
- Q: Suppose $f$ is defined on a closed interval $[a,b]$. Define continuity at the left-hand endpoint, $a$. Also define continuity at the right-hand endpoint, $b$.  
- A: We say $f$ is continuous at the left-hand endpoint, $a$, if and only if $$\lim_{x\to a+} f(x) = f(a);$$ we say $f$ is continuous at the right-hand endpoint, $b$, if and only if $$\lim_{x\to b-} f(x) = f(b).$$

## Differentiation

- Q: Evaluate $$\lim_{x\to \infty}(1+2^x)^{1/x}.$$ 
- A: If $L = \lim_{x\to \infty}(1+2^x)^{1/x},$then $$\ln L =\lim_{x\to \infty}\ln((1+2^x)^{1/x}).$$Using L'H\^opital's rule twice, we find$$\ln L =\lim_{x\to \infty}\frac{(\ln(2))^2\cdot 2^x}{\ln(2)\cdot 2^x} = \ln(2).$$So $L = 2$.
- Q: Suppose $y = (\ln(x))^x.$ What is $\frac{dy}{dx}$? 
- A: We know $y = (\ln(x))^x$, so $\ln(y) = x\ln(\ln(x))$. Because $\frac{d}{dx}\ln(y) = \frac{1}{y}\frac{dy}{dx},$ we can find\begin{align*}\frac{dy}{dx} &= y\cdot\frac{d}{dx}[\ln(y)]\\&= (\ln(x))^x \cdot \frac{d}{dx} [x\ln(\ln(x))]\\&=(\ln(x))^x\cdot\left(\ln(\ln(x))+x\cdot\frac{1}{\ln(x)}\cdot\frac{1}{x}\right)\\&=(\ln(x))^x\cdot\left(\ln(\ln(x))+\frac{1}{\ln(x)}\right).\end{align*}
- Q: Evaluate $$\lim_{h\to 0} \frac{\arccos(1/2 + h) - \pi/3}{h}.$$ 
- A: Because $\arccos(1/2) = \pi/3$, we have $$\lim_{h\to 0} \frac{\arccos(1/2 + h) - \pi/3}{h} = \lim_{h\to 0} \frac{\arccos(1/2 + h) - \arccos(1/2)}{h}.$$ This is the tangent line to $\arccos(x)$ at $x=1/2$. So$$\lim_{h\to 0} \frac{\arccos(1/2 + h) - \arccos(1/2)}{h} = \left[\frac{d}{dx}[\arccos(x)]\right]_{x=1/2}.$$ Recalling$\frac{d}{dx}[\arccos(x)] = -\frac{1}{\sqrt{1-x^2}}$, we have$$\left[\frac{d}{dx}[\arccos(x)]\right]_{x=1/2} =-\sqrt{\frac{4}{3}}.$$
- Q: What is $\frac{d}{dx}[a^{u(x)}]$? 
- A: Recall $$\frac{d}{dx}[a^u(x)] = \ln(a)a^{u(x)}\frac{du}{dx}.$$ Here's why. Let $y = a^{u(x)}$. Then $$\ln(y) = u(x)\ln(a).$$ Implicitly differentiating w.r.t. $x$,$$\frac{1}{y}\frac{dy}{dx} = \ln(a)\frac{du}{dx}.$$ whence $$\frac{dy}{dx} = y\ln(a)\frac{du}{dx} = \ln(a)a^{u(x)}\frac{du}{dx}.$$
- Q: What is the derivative (with respect to $x$) of $\theta = \arctan(x)$? 
- A: Well, if $\arctan(x) = \theta$, then $x = \tan(\theta)$. Applying $\frac{d}{dx}$ to both sides of the equation, we find\begin{align*}1 &= \frac{d}{dx}\tan(\theta)\\&= \frac{d}{d\theta}\tan(\theta)\frac{d\theta}{dx}\text{ (by the chain rule)}\\&= \frac{1}{\cos^2(\theta)}\frac{d\theta}{dx}\\&= \frac{1}{\cos^2(\arctan(x))}\frac{d\theta}{dx}.\end{align*}Whence $\frac{d\theta}{dx} =\cos^2(\arctan(x)) = \frac{1}{x^2 +1}.$
- Q: What is the derivative (with respect to $x$) of $\theta = \arcsin(x)$? 
- A: Well, if $\arcsin(x) = \theta$, then $x = \sin(\theta)$. Applying $\frac{d}{dx}$ to both sides of the equation, we find\begin{align*}1 &= \frac{d}{dx}\sin(\theta)\\&= \frac{d}{d\theta}\sin(\theta)\frac{d\theta}{dx}\text{ (by the chain rule)}\\&= \cos(\theta) \frac{d\theta}{dx}\\&= \cos(\arcsin(x)) \frac{d\theta}{dx}.\end{align*}Whence $\frac{d\theta}{dx} =\frac{1}{\cos(\arcsin(x))}= \frac{1}{\sqrt{1-x^2}}.$
- Q: What is the derivative (with respect to $x$) of $\theta = \arccos(x)$? 
- A: Well, if $\arccos(x) = \theta$, then $x = \cos(\theta)$. Applying $\frac{d}{dx}$ to both sides of the equation, we find\begin{align*}1 &= \frac{d}{dx} \cos(\theta)\\ &= \frac{d}{d\theta}\cos(\theta)\frac{d\theta}{dx}\text{ (by the chain rule)}\\ &= -\sin(\theta) \frac{d\theta}{dx}\\ &= -\sin(\arccos(x)) \frac{d\theta}{dx}.\end{align*}Whence $\frac{d\theta}{dx} =\frac{-1}{\sin(\arccos(x))}= \frac{-1}{\sqrt{1-x^2}}.$
- Q: State the Extreme Value Theorem. 
- A: Suppose $f:[a,b] \to \RR$ is a continuous function. There exist points $c$ and $d$ in $[a,b]$ such that $$f(c)\leq f(x)\leq f(d)$$ holds true for every $x \in [a,b]$.
- Q: State Bolzano's theorem. 
- A: Suppose $f:[a,b] \to \RR$ is a continuous function. If $f(a)$ and $f(b)$ have opposite signs, then there exists a point $x_0$ in $(a,b)$ such that $f(x_0) = 0$.
- Q: State the Intermediate Value theorem. 
- A: Suppose $f:[a,b] \to \RR$ is a continuous function. Let $y_0$ be a real number lying between $f(a)$ and $f(b)$, i.e. with$$f(a)\leq y_0 \leq f(b) \text{ or } f(b) \leq y_0 \leq f(a).$$There is at least one $c$, with $$a\leq c \leq b, \text{ such that } y_0 = f(c).$$I postulate that the IVT is equivalently stated:\begin{align*}f:[a,b] \to \RR \text{ is cts. and } y_0 \in (f(a),(f(b))\\\implies \text{there is } c \in (a,b) \text{ s.th. } f(c) = y_0.\end{align*}
- Q: State and prove Brouwer's fixed-point theorem. 
- A: If $f:[0,1]\to[0,1]$ is cts. there is $c \in [0,1]$ s.th. $f(c) = c$.
    - Proof. If $f(0) = 0$ or $f(1) = 1$, the conclusion is immediate, so assume $f(0) \in (0,1]$ and $f(1) \in [0,1)$. Define the cts. function$$g(x) = f(x) -x.$$ We can see that $$g(0) = f(0) >0 \text{ and } g(1) = f(1) - 1 < 0.$$ By Bolzano's theorem, there must be a point $c \in [a,b]$ such that $g(c) = 0$. So $f(c) - c =0$ or $f(c) = c$.
- Q: For a real-valued function $f$ of a single real variable, the derivative of $f$ is the function $f'$ whose value at $x$ is what? 
- A: $$f'(x) = \lim_{h\to 0}\frac{f(x+h)-f(x)}{h},$$ provided the limit exists.
- Q: What is the relation between continuity at a point and differentiability at a point? 
- A: If $f$ is not continuous at a point $a$, them $f$ is not differentiable at $a$. Equivalently,$$f \text{ is diff'ble at } a \implies f \text{ is cts. at } a.$$
- Q: Define Leibniz notation. 
- A: The difference quotient used in the definition of the derivative is a change in $f$ divided by a change in $x$; that is, we can write$$f'(x) = \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x} = \lim_{\Delta x \to 0} \frac{\Delta f}{\Delta x} = \frac{df}{dx}.$$
- Q: What is the derivative of a sum? 
- A: $$(f+g)'(x) = f'(x) + g'(x)$$
- Q: What is the derivative of a constant multiple? 
- A: $$(kf)'(x) = kf'(x)$$
- Q: What is the derivative of a product? 
- A: The product rule states: $$(fg)'(x) = f'(x)g(x) + f(x)g'(x).$$
- Q: What is the derivative of a quotient? 
- A: The quotient rule states: $$\left(\frac{f}{g}\right)'(x) = \frac{f'(x)g(x) - f(x)g'(x)}{[g(x)]^2}.$$
- Q: What is the derivative of a composite function? 
- A: The chain rule states: $$(f\circ u)'(x) = f'(u(x))\cdot u'(x).$$
- Q: What is the derivative of an inverse function? 
- A: The inverse function rule states that if $f^{-1}$ is the inverse of $f$, and $f$ has a nonzero derivative at $x_0$, then $f^{-1}$ has a derivative at $y_0 = f(x_0)$, and $$(f^{-1})'(y_0) = \frac{1}{f'(x_0)}.$$ In Leibniz notation, $$\frac{dx}{dy} = \frac{1}{\frac{dy}{dx}}.$$
- Q: Given a function, $y = f(x)$, use implicit differentiation to find the derivative of the inverse function, $f^{-1}(y) = x$. 
- A: If $y = f(x)$, then $f^{-1}(y) = x$. Differentiating w.r.t. $x$,$$\frac{d}{dx}(f^{-1}(y)) = \frac{d}{dx}(x) = 1.$$ The chain rule implies $$\frac{d}{dx}(f^{-1}(y)) = \frac{d}{dy}(f^{-1}(y))\frac{dy}{dx},$$ whence $\frac{d}{dy}(f^{-1}(y)) = \frac{1}{\frac{dx}{dy}}.$
- Q: Write the following differential in terms of $du$:$$d(k)$$ 
- A: $$d(k) = 0$$
- Q: Write the following differential in terms of $du$:$$d(u^k)$$ 
- A: It can be proven that $$d(u^k) = ku^{k-1}du.$$Of course, as a special case, $$d(u^0) = 0u^{-1}du = 0.$$
- Q: Write the following differential in terms of $du$:$$d(e^u)$$ 
- A: $$d(e^u) = e^udu$$
- Q: Write the following differential in terms of $du$:$$d(a^u)$$ 
- A: $$d(a^u) = (\log (a))a^udu$$
- Q: Write the following differential in terms of $du$:$$d(\log (u))$$ 
- A: $$d(\log (u)) = \frac{1}{u}du$$
- Q: Write the following differential in terms of $du$:$$d(\log_a (u))$$where $a \neq 1$. 
- A: $$d(\log_a (u)) = \frac{1}{\log (a)} \cdot \frac{1}{u}du$$
- Q: Write the following differential in terms of $du$:$$d(\sin(u))$$ 
- A: $$d(\sin (u)) = \cos (u) du$$
- Q: Write the following differential in terms of $du$:$$d(\cos (u))$$ 
- A: $$d(\cos (u)) = -\sin (u) du $$
- Q: Write the following differential in terms of $du$:$$d(\tan (u))$$ 
- A: $$d(\tan (u)) = \sec^2 (u) du$$
- Q: Write the following differential in terms of $du$:$$d(\cot (u))$$ 
- A: $$d(\cot (u)) =-\csc^2(u)du$$
- Q: Write the following differential in terms of $du$:$$d(\sec(u))$$ 
- A: $$d(\sec (u)) =\sec(u)\tan(u)du$$
- Q: Write the following differential in terms of $du$:$$d(\csc(u))$$ 
- A: $$d(\csc(u) = -\csc(u)\cot(u)du$$
- Q: Write the following differential in terms of $du$:$$d(\arcsin(u))$$ 
- A: $$d(\arcsin(u)) = \frac{du}{\sqrt{1-u^2}}$$
- Q: Write the following differential in terms of $du$:$$d(\arccos(u))$$ 
- A: $$d(\arccos(u)) = -\frac{du}{\sqrt{1-u^2}}$$
- Q: Write the following differential in terms of $du$:$$d(\arctan(u))$$ 
- A: $$d(\arctan(u)) = \frac{du}{1+u^2}$$
- Q: What is the equation of the line tangent to the graph of $y = f(x)$ at the point $x = a$? 
- A: The equation is $$T_1(x) = f'(a)(x-a) + f(a),$$the first order Taylor Expansion of $f(x)$ about $x=a$.
- Q: Let $f: D \subseteq \RR \to \RR$. For $x_0 \in D$, suppose $f(x_0)$ and $f'(x_0)$ are known. If $|\Delta x|<<1$, what is an approximate value for $f(x_0 + \Delta x)$? 
- A: With $\Delta y = f'(x_0)\Delta x$, we know$$f(x_0 + \Delta x) \approx f(x_0) + \Delta y = f(x_0) +f'(x_0)\Delta x.$$

## Basic Analysis

- Q: State the Implicit Function Theorem. 
- A: If $P_0 = (x_0,y_0)$ satisfies the equation $f(x,y) = c$ and both partial derivatives $f_x$ and $f_y$ are cts. in a neighborhood of $P_0$ (with $f_y \neq 0$ at $P_0$), then there exists a unique differentiable function, $$y = g(x),$$ that satisfies both $$f(x,y) = c \text{ and }y_0 = g(x_0).$$ Furthermore,$$y' = \frac{-f_x}{f_y}.$$
- Q: Describe the properties of the first derivative. 
- A: 
    - Where $f'(x) > 0$, the slope is positive---the function is increasing.
    - Where $f'(x) < 0$, the slope is negative---the function is decreasing.
    - Where $f'(x) = 0$, the function has a horizontal tangent line.
    - Where $f'(x)$ does not exist, the function could have a vertical tangent line or it might not be differentiable at that point.
- Q: Describe the properties of the second derivative. 
- A: 
    - Where $f''(x) > 0$, the curve is concave up---the curve lies above its tangent line. 
    - Where $f''(x) < 0$, the curve is concave down---the curve lies below its tangent line.
    - $f''(x) = 0$ or $f''(x)$ D.N.E. are necessary, yet not sufficient, conditions for points of inflection.
- Q: State Rolle's Theorem. 
- A: Let $f:[a,b] \to \RR$ be a cts. function, which is diff'ble at every point in $(a,b)$. If $f(a) = f(b)$, then there exists a point $c$ in $(a,b)$ at which $f'(c) = 0$.
- Q: State the Mean-Value Theorem. 
- A: Let $f:[a,b] \to \RR$ be a cts. function, which is diff'ble at every point in $(a,b)$. There exists a point $c$ in $(a,b)$ at which$$f'(c) = \frac{f(b)-f(a)}{b-a}$$.
- Q: Let $f$ be a function, cts. on the interval $I$. If $f'(x) = 0$ for all $x \in I$, then (describe $f$) 
- A: for some constant $k$, we know $$f(x) = k$$ for all $x \in I$.
- Q: Let $f$ be a function, cts. on the interval $I$. Define a local minimum of $f$. 
- A: We say $(c,f(c))$ is a local minimum if and only if there exists some subinterval, $$U \subseteq I,$$ such that $$f(c)\leq f(x) \text{ for all }x \in U.$$
- Q: Let $f$ be a function, cts. on the interval $I$. Define the absolute minimum of $f$. 
- A: There exists $c$ in $I$ such that $f(c)\leq f(x)$ for all $x \in I$ if and only if $(c,f(c))$ is a absolute minimum.
- Q: Let $f$ be a function, cts. on the interval $I$. Define a local maximum of $f$. 
- A: We say $(c,f(c))$ is a local maximum if and only if there exists some subinterval, $$U \subseteq I,$$ such that $$f(c)\geq f(x) \text{ for all }x \in U.$$
- Q: Let $f$ be a function, cts. on the interval $I$. Define the absolute maximum of $f$. 
- A: There exists $c$ in $I$ such that $f(c)\leq f(x)$ for all $x \in I$ if and only if $(c,f(c))$ is a absolute minimum.
- Q: Let $f$ be a function, cts. on the interval $I$. Define an extremum for the function $f$. 
- A: An extremum of $f$ is the ordered pair $(c,f(c))$ if and only if $(c,f(c))$ is a local maximum or minimum of $f$.
- Q: What is the Second Derivative Test? 
- A: \begin{align*}f'(c) = 0 \text{ and } f''(c) > 0 &\implies (c,f(c)) \text{ is a local minimum;}\\f'(c) = 0 \text{ and } f''(c) < 0 &\implies (c,f(c)) \text{ is a local maximum.}\end{align*}
- Q: What are the three possibilities for the location of the absolute extrema for a cts. function $f:[a,b] \to \RR$? 
- A: An absolute extremum will occur
    - at a point $(c,f(c))$ such that $f'(c) = 0$,
    - at a point $(c,f(c))$ such that $f'(c)$ fails to exist, or
    - at either $(a,f(a))$ or $(b,f(b))$, where $a$ and $b$ are the endpoints of the domain.
- Q: State the $n^{th}$ derivative test. 
- A: Assume that the function $f(x)$ is smooth, and let $x = x_0$ be a critical point of $f$. Find the smallest integer $n$ such that $f^{(n)}(x_0) \neq 0$. If $n$ is even and $$f^{(n)}(x_0) > 0,$$ then the graph lies about its tangent line and $f$ has a local minimum at $x_0$; if $n$ is even and $$f^{(n)}(x_0) < 0,$$ then the graph lies below its tangent line and $f$ has a maximum at $x_0$; if $n$ is odd, then $f$ has neither a local minimum nor a local maximum at $x_0$.

## Integration

- Q: Evaluate $\int_0^{1/6} \frac{\sin^{-1}(3t)}{\sqrt{1-9t^2}}dt$. 
- A: Let $u(t) = \sin^{-1}(3t)$. Then $$du = \frac{1}{\sqrt{1-(3t)^2}}\cdot 3dt.$$ With $u(0) = \sin^{-1}(0) = 0$ and $u(1/6) = \sin^{-1}(1/2) = \pi/6$, we can express the integral entirely in terms of $u$:\begin{align*}\int_0^{1/6} \frac{\sin^{-1}(3t)}{\sqrt{1-9t^2}}dt &=\int_0^{\pi/6} u\cdot \frac{du}{3}\\&= \frac{\pi^2}{216}.\end{align*}
- Q: Which of the following are not approximation methods?
    - Newton’s Method
    - Average rate of change
    - Linearization
    - Riemann Sum
- A: Average rate of change is NOT an approximation method.
- Q: The expression $$\sum_{i=1}^3 g\left(2+\frac{2i}{3}\right)\cdot\frac{2}{3}$$ is a left endpoint approximation for which integral? 
- A: \begin{align*}&\sum_{i=1}^3 g\left(2+\frac{2i}{3}\right)\cdot\frac{2}{3} \\&=g\left(\frac{8}{3}\right)\cdot\frac{2}{3} +g\left(\frac{10}{3}\right)\cdot\frac{2}{3}+g\left(\frac{12}{3}\right)\cdot\frac{2}{3}\\&\approx \int_{8/3}^{14/3} g(x)dx.\end{align*}
- Q: If $\mathbf{x}(t)$ is a parameterized curve and $\mathbf{v}(t)$ is its velocity, $\frac{d\mathbf{x}}{dt}$, the length of the curve traced out between $t = a$ and $t = b$ is given by 
- A: $$s = \int_a^b|\mathbf{v}(t)|dt.$$
- Q: An antiderivative (or indefinite integral) of a function $f(x)$ is a function $F(x)$ whose derivative is $f(x)$. Because $$\frac{d}{dx}\left[x^n\right] = nx^{n-1} \text{ and } \frac{d}{dx}\left[\log(x)\right] = x^{-1}$$ what is$$\int x^n dx?$$ 
- A: \begin{equation*}\int x^n dx =\begin{cases}\frac{x^{n+1}}{n+1} &\text{if } n \neq -1\\\log|x| &\text{if } n =-1\\\end{cases}\end{equation*}
- Q: Suppose $F(x)$ is an antiderivative of $f(x)$. If $a$ and $b$ are constants, what's $$\int f(ax+b) dx?$$ 
- A: $$\int f(ax+b) dx = \frac{1}{a}F(ax+b)+c.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate$$\int kdu.$$ 
- A: For any arbitrary constant $c$, we find the antiderivatives $$\int kdu = ku + c.$$ This follows from $$d(ku) = k\cdot du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int u^kdu$$ 
- A: For any arbitrary constant $c$, we find the antiderivative\begin{equation*}\int u^kdu = \begin{cases} \frac{u^{k+1}}{k+1} + c &\text{if } k \neq -1\\ \log|k|+ c &\text{if } k =-1\end{cases}\end{equation*}
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int e^udu$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int e^udu = e^u + c.$$ This follows from $$d(e^u + c) = k\cdot du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$) and $a>0$ evaluate: $$\int a^udu$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int a^udu = \frac{1}{\log(a)}a^u + c.$$ This follows from $$d(a^u + c) = \log(a)a^udu.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \sin(u) du$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int \sin(u) du = -\cos(u) + c.$$ This follows from $$d(\cos(u)+c) = -\sin(u) du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \cos(u)du$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int \cos(u)du= \sin(u)+ c.$$ This follows from $$d(\sin(u)+c) = \cos(u) du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \sec^2(u)du$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int \sec^2(u)du = \tan(u) + c.$$ This follows from $$d(\tan(u) + c) = \frac{1}{\cos^2(u)} du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \csc^2(u)du$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int \csc^2(u)du = -\cot(u)+c.$$ This follows from $$d(\cot(u) + c) = -\frac{1}{\sin^2(u)}du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \sec(u)\tan(u)du$$ 
- A: Write $$\int \sec(u)\tan(u)du = \int \frac{1}{\cos(u)}\frac{\sin(u)}{\cos(u)}du,$$ then, considering $\sin(u)du = -d(\cos(u))$, integrate$$\int \frac{-d(\cos(u)}{\cos^2(u)} = \frac{1}{\cos(u)} +c.$$So, for an arbitrary constant $c$, we find $$\int\sec(u)\tan(u)du = \sec(u) + c.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \csc(u)\cot(u)du$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int \csc(u)\cot(u)du = -\csc(u) + c.$$ This follows from $$d(\csc(u)+c) = -\frac{\cos(u)}{\sin^2(u)} du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \frac{du}{\sqrt{1-u^2}}$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int \frac{du}{\sqrt{1-u^2}} = \arcsin(u) + c.$$ This follows from $$d(\arcsin(u)+c) = \frac{1}{\sqrt{1-u^2}} du.$$
- Q: With $u$ as the variable of integration (possibly a diff'ble function of $x$), evaluate: $$\int \frac{du}{1+u^2}$$ 
- A: For any arbitrary constant $c$, we find the antiderivative $$\int \frac{du}{1+u^2} = \arctan(u) + c.$$ This follows from $$d(\arctan(u) + c) = \frac{1}{1+u^2}du.$$
- Q: Evaluate $\int_0^{1/6} \frac{\sin^{-1}(3t)}{\sqrt{1-9t^2}}dt$. 
- A: Let $u(t) = \sin^{-1}(3t)$. Then $$du = \frac{1}{\sqrt{1-(3t)^2}}\cdot 3dt.$$ With $u(0) = \sin^{-1}(0) = 0$ and $u(1/6) = \sin^{-1}(1/2) = \pi/6$, we can express the integral entirely in terms of $u$:\begin{align*}\int_0^{1/6} \frac{\sin^{-1}(3t)}{\sqrt{1-9t^2}}dt &=\int_0^{\pi/6} u\cdot \frac{du}{3}\\&= \frac{\pi^2}{216}.\end{align*}
- Q: Which of the following are not approximation methods?
    - Newton’s Method
    - Average rate of change
    - Linearization
    - Riemann Sum
- A: Average rate of change is NOT an approximation method.
- Q: The expression $$\sum_{i=1}^3 g\left(2+\frac{2i}{3}\right)\cdot\frac{2}{3}$$ is a left endpoint approximation for which integral? 
- A: \begin{align*}&\sum_{i=1}^3 g\left(2+\frac{2i}{3}\right)\cdot\frac{2}{3} \\&=g\left(\frac{8}{3}\right)\cdot\frac{2}{3} +g\left(\frac{10}{3}\right)\cdot\frac{2}{3}+g\left(\frac{12}{3}\right)\cdot\frac{2}{3}\\&\approx \int_{8/3}^{14/3} g(x)dx.\end{align*}
- Q: If $\mathbf{x}(t)$ is a parameterized curve and $\mathbf{v}(t)$ is its velocity, $\frac{d\mathbf{x}}{dt}$, the length of the curve traced out between $t = a$ and $t = b$ is given by 
- A: $$s = \int_a^b|\mathbf{v}(t)|dt.$$
- Q: The differential of the product of the functions $u$ and $v$ is $$d(uv) = du\cdot v + u\cdot dv.$$ Equivalently, $$u\cdot dv = d(uv) - v \cdot du.$$ State the formula for integration by parts. 
- A: We find $$\int u\cdot dv = uv - \int v \cdot du.$$
- Q: If $u$ is the variable of integration and the integral contains $\sqrt{a^2-u^2}$, what trigonometric substitution could be helpful? 
- A: Let $u = a\sin(\theta)$ and $du = a\cos(\theta) d\theta$. 
- Q: If $u$ is the variable of integration and the integral contains $\sqrt{a^2+u^2}$, what trigonometric substitution could be helpful? 
- A: $u = a\tan(\theta)$ and $du = a\sec^2(\theta) d\theta$. 
- Q: If $u$ is the variable of integration and the integral contains $\sqrt{u^2-a^2}$, what trigonometric substitution could be helpful? 
- A: Let $u = a\sec(\theta)$ and $du = a\sec(\theta)\tan(\theta) d\theta$.
- Q: To find the algebraic area under $$f\colon[a,b] \to \RR.$$ Consider$n$ rectangular strips, each of width $$\Delta x = \frac{b-a}{n}.$$ Let the height of each rectangle be $f(x)$ at the right hand endpoint of the rectangle's base. What is the sum of the areas of these rectangles? 
- A: \begin{align*}S_n &=\\&\Delta x[f(a+\Delta x)+ f(a+2\Delta x)+ \cdots\\&+ f(a+(n-1)\Delta x ) + f(b)],\end{align*} a Riemann Sum. As $n \to \infty$, we find that $S_n$ approaches the algebraic area under the function $f$ (between the lines $x=a$ and $x=b$).
- Q: What is a definite integral? 
- A: The definite integral is the algebraic area under a real-valued function $f(x)$, between two lines $x=a$ and $x=b$. This area is denoted by $$\int_a^b f(x)dx,$$ and defined by the limit of a Riemann sum.
- Q: State the FTC (Part I). 
- A: If $f\colon[a,b] \to \RR$ be a cts. function and $F(x)$ be an antiderivative of $f(x)$, then $$\int_a^b f(x)dx = \left[F(x)\right]_a^b = F(b) - F(a).$$
- Q: State the FTC (Part II). 
- A: If $f\colon[a,b] \to \RR$ be a cts. function, then, for any $x \in [a,b]$, $$\frac{d}{dx}\int_a^t f(t)dt = f(x).$$
- Q: Suppose $a(x)$ and $b(x)$ are functions of $x$. What is $$\frac{d}{dx}\int_{a(x)}^{b(x)}f(t)dt?$$ 
- A: Let $F(t)$ be an antiderivative of $f(t)$. Then\begin{align*}\frac{d}{dx}\left[\int_{a(x)}^{b(x)}f(t)dt\right] &= \frac{d}{dx}\left[F(b(x))-F(a(x))\right] &\text{by the FTC I,}\\&=\frac{dF}{db}\frac{db}{dx}-\frac{dF}{da}\frac{da}{dx} &\text{by the Chain Rule,}\\&=f(b(x))\frac{db}{dx} - f(a(x))\frac{da}{dx} &\text{as $\frac{dF}{dt}= f(t)$.}\end{align*}
- Q: Regarding definite integral rules, what is the relation between $\int_a^b f(x)dx$ and $\int_b^a f(x)dx$? 
- A: It can be proven that $$\int_a^b f(x)dx = -\int_b^a f(x)dx.$$
- Q: Regarding definite integral rules, what is $\int_a^a f(x)dx$? 
- A: Consider the fact that $$\int_a^b f(x)dx = -\int_b^a f(x)dx.$$ Letting $a=b$, we find $\int_a^a f(x)dx = -\int_a^a f(x)dx$. So $$\int_a^a f(x)dx = 0.$$
- Q: Regarding definite integral rules, Assuming $a \leq b \leq c$, what is $$\int_a^b f(x)dx + \int_b^c f(x)dx?$$ 
- A: It can be proven that $$\int_a^b f(x)dx + \int_b^c f(x)dx = \int_a^c f(x)dx.$$
- Q: Regarding definite integral rules, for a constant $k$, what's $$\int_a^b kf(x)dx?$$ 
- A: It can be proven that $$\int_a^b kf(x)dx = k\int_a^b f(x)dx.$$
- Q: Regarding definite integral rules, what is $$\int_a^b [f(x)\pm g(x)]dx?$$ 
- A: It can be proven that $$\int_a^b [f(x)\pm g(x)]dx = \int_a^b f(x)dx \pm \int_a^b g(x)dx.$$
- Q: Regarding definite integral rules, if $$f(x) \leq g(x)\text{ for all } x \in [a,b],$$ what is the relation between $\int_a^b f(x)dx$ and $\int_a^b g(x)dx$? 
- A: It can be proven that $$\int_a^b f(x)dx \leq \int_a^b g(x)dx.$$
- Q: State the mean-value theorem for integrals. 
- A: If $f\colon [a,b] \to \RR$ is a cts. function, there exists $c \in (a,b)$ such that $$\int_a^b f(x)dx = f(c)(b-a).$$
- Q: What is the area of an infinitesmal circular sector of angle $d\theta$ and radius $r$? 
- A: A circle of radius $r$ has area $\pi r^2$. So the sum of all of the infinitesmal circular sectors (of a constant radius, from angle $0$ to $2\pi$) should have the area $\pi r^2$. We solve for $\alpha$,\begin{align*}\pi r^2 &= \int_0^{2\pi} \alpha r^2d\theta\\&= \alpha r^2 \cdot 2\pi\end{align*}We find $\alpha = \frac{1}{2}$; thus the area of an infinitesmal circular sector is $$\frac{1}{2}r^2d\theta.$$
- Q: When we rotate a portion of a curve, $y = f(x)$ from $x=a$ to $x=b$, around the $x$-axis we enclose a solid of revolution. What is its volume? 
- A: Consider thin disks normal to the $x$-axis, whose radius is $f(x)$ and height is $dx$. The volume of each disk is $$dV = \pi[f(x)]^2dx.$$ The volume of the solid is the sum of the volume of the disks, so$$V = \int_a^b \pi[f(x)]^2dx.$$
- Q: When we rotate a portion of a curve, $x = g(y)$ from $y=a$ to $y=b$, around the $y$-axis we enclose a solid of revolution. What is its volume? 
- A: Consider thin disks normal to the $y$-axis, whose radius is $g(y)$ and height is $dy$. The volume of each disk is $$dV = \pi[g(y)]^2dy.$$ The volume of the solid is the sum of the volume of the disks, so$$V = \int_a^b \pi[g(y)]^2dy.$$
- Q: Prove that the natural logarithm is an antiderivative of the function $g(x) = \frac{1}{x}$. 
- A: We'll prove that $\frac{d}{dx}[\ln(x)] = \frac{1}{x}$. Let $y = \ln(x)$. So $x = e^y$. (The two previous sentences are equivalent.) Implicitly differentiating w.r.t. $x$,$$1 =e^y\frac{dy}{dx} \implies \frac{dy}{dx} = \frac{1}{e^y} = \frac{1}{x}.$$
- Q: Define the natural logarithm as an integral. 
- A: The natural logarithm is an antiderivative of $g(t) = \frac{1}{t}$. So\begin{align*}\int_1^x g(t)dt &= \log(x) - \log(1) &\text{by the FTC I,}\\&= \log(x) &\text{because $\log(1) = 0$, i.e.,$e^0 =1$.}\end{align*}
- Q: State L'H\^opital's Rule. 
- A: If $f(x)$ and $g(x)$ are diff'ble functions in an open interval, $I$, containing $a$ (except possibly at $a$ itself) such that $g'(x) \neq 0$ for all $x\neq a$ in $I$, and $f(a) = g(a) = 0$, then $$\lim_{x\to a} \frac{f(x)}{g(x)} = \lim_{x\to a} \frac{f'(x)}{g'(x)}$$ provided that the limit on the right exists (or is possibly indeterminate).
- Q: Define $$\int_a^\infty f(x)dx.$$ 
- A: We define $$\int_a^\infty f(x)dx = \lim_{b\to\infty} \int_a^b f(x)dx.$$ The integral converges if and only if the limit exists.
- Q: The length of a smooth curve (or an arc) is the sum of the infinitesmal displacements along its breadth. For a curve $y=f(x)$ in the plane, what is the arc length from $x=a$ to $x=b$? 
- A: Let $ds = \sqrt{dx^2+dy^2}$. The arc length is\begin{align*}S &= \int_a^b ds\\&= \int_a^b \sqrt{dx^2+dy^2}\\&= \int_a^b \sqrt{1+\left(\frac{dy}{dx}\right)^2}\cdot dx.\end{align*} So we must differentiate, then integrate!
- Q: The derivative of every exponential function of the form $f(x) = a^x$ (with $a>0$) is equal to a multiple of itself:\begin{align*}f'(x) &= \lim_{h\to 0}\frac{f(x+h)-f(x)}{h}\\&= \lim_{h\to 0}\frac{a^{x+h} -a^x}{h}\\&=a^x \lim_{h\to 0}\frac{a^h-1}{h}\end{align*}Keeping in mind the above calculation, define the base of the natural exponential function. 
- A: If we can find the value of $a$ such that $\frac{a^h-1}{h} = 1$, then $f'(x) = f(x)$. So let's define $e$ such that $$\lim_{h\to 0}\frac{e^h-1}{h} = 1.$$
- Q: Considering $$\lim_{h\to 0}\frac{e^h-1}{h} = 1,$$ approximate $e$. Also give a numerical approxiamation. 
- A: If $h$ is very small, then $$e^h-1 \approx h\implies e^h \approx 1+h \implies e \approx (1+h)^{1/h}.$$ The value of $e$ is about $2.718$.
- Q: What is the slope of the natural exponential function, $f(x) = e^x$, at $x = 0$? Why is this special? 
- A: The slope of the natural exponential function at $x =0$ is $1$. No exponential function, distinct from $e^x$, has a slope of $1$ at $x=0$.
- Q: Define $$\int_{-\infty}^b f(x)dx.$$ 
- A: We define $$\int_{-\infty}^b f(x)dx = \lim_{a\to -\infty} \int_a^b f(x)dx.$$ The integral converges if and only if the limit exists.
- Q: Define $$\int_{-\infty}^\infty f(x)dx.$$ 
- A: For any $c \in \RR$, we define $$\int_{-\infty}^\infty f(x)dx = \int_{-\infty}^c f(x)dx + \int_c^{\infty} f(x)dx.$$ The integral converges if and only if both the right hand integrals converge.
- Q: Consider a function $f:D \to \RR$, where $D \subseteq \RR$. If $z$ is on the boundary of $D$, what is $$\int_{z}^b f(x)dx?$$ 
- A: For $a \in D$, we define $$\int_{z}^b f(x)dx = \lim_{a \to z} \int_a^b f(x)dx.$$ The integral converges if and only if the limit exists.

- Q: Using the partial fraction decomposition$$\frac{1}{(u-a)(u-b)} = \frac{1}{a-b}\left(\frac{1}{u-a}-\frac{1}{u-b}\right)$$ find a primitive of the secant function. 
- A: \begin{align*}\int \sec\theta d\theta &= \int\frac{d\theta}{\cos\theta}\\&= \int\frac{\cos\theta d\theta}{\cos^2\theta}\\&=\int \frac{\cos\theta d\theta}{1-\sin^2\theta}\\&=\int \frac{du}{1-u^2} &\text{substituting} u = \sin\theta\\&=\int \frac{1}{2}\left(\frac{1}{1-u}+\frac{1}{1+u}\right)du &\text{by partial fractions}\\&=\frac{1}{2}\big(-\ln|1-u|+\ln|1+u|\big)\\&=\frac{1}{2}\ln\left|\frac{1+u}{1-u}\right|\\&= \frac{1}{2}\ln\left|\frac{1+\sin\theta}{1-\sin\theta}\right| &\text{back-substituting}\\&= \frac{1}{2}\ln\left|\frac{(1+\sin\theta)^2}{1-\sin^2\theta}\right| &\text{multiplying by }\frac{1+\sin\theta}{1+\sin\theta}\\&= \ln\left|\sqrt{\frac{(1+\sin\theta)^2}{\cos^2\theta}}\right| &\text{log rule and trig identity}\\& = \ln\left|\frac{1+\sin\theta}{\cos\theta}\right|\\&= \ln|\sec\theta+\tan\theta|.\end{align*}

## Taylor series

- Q: When does the power series$\sum_{n=0}^{\infty}a_nx^n$ (absolutely) converge? 
- A: We'll find all $x$ such that $\sum_{n=0}^{\infty}|a_nx^n|$ converges. By the ratio test, the series will converge absolutely if$$\lim_{n\to\infty}\left|\frac{a_{n+1}x^{n+1}}{a_nx^n}\right| = \lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|\cdot|x| < 1.$$ Thus we have the requirement $$|x| < \frac{1}{\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|}.$$ Letting $L =\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|$, we describe:\begin{align*}L = 0 &\implies \sum |a_nx^n| \text{ conv. for all } x \in \RR\\L = \infty &\implies \sum |a_nx^n| \text{ conv. iff } x = 0\\\text{else}&\implies \sum |a_nx^n| \text{ conv. iff } |x| < \frac{1}{L}\\&\implies \sum a_nx^n \text{ div. iff } |x| > \frac{1}{L}\\\end{align*}
- Q: Knowing $$\int_{-\infty}^{\infty}e^{-x^2}dx = \sqrt{\pi},$$ find $$\int_{0}^{\infty}x^2e^{-x^2}dx$$ 
- A: I don't know how to do this.
- Q: Suppose $\sum_{n=0}^{\infty}a_nx^n$ converges whenever $x \in I$. List three important facts about the function $f\colon I \to \RR$ defined by $$f(x) = \sum_{n=0}^{\infty}a_nx^n.$$ 
- A: \begin{description}
    - continuous: $f$ is continuous on its domain.
    - diff'ble: The function $f$ is differentiable and$$f'(x) = \sum_{n=0}^{\infty}\frac{d}{dx}\left[a_nx^n\right] =\sum_{n=1}^{\infty}na_nx^{n-1}.$$
    - intg'ble: The function $f$ is integrable and$$\int f(x)dx = \sum_{n=0}^{\infty}\int a_nx^ndx=\sum_{n=0}^{\infty}\frac{a_n}{n+1}x^{n+1}.$$\end{description}
- Q: Assuming the function $f$ has a power series representation (centered at $0$), what are the Taylor coefficients of the power series? Will any other coefficients do the trick? 
- A: We have $f(x) = a_0 + a_1x + a_2x^2 + a_3x^3 + \cdots$. Finding the value of the n-th derivative of $f$ at $x = 0$ yields$$a_n = \frac{f^{(n)}(0)}{n!}.$$ The power series $$f(x) = \sum_{n=1}^\infty\frac{f^{(n)}(0)}{n!}x^n$$ is called the Taylor series (centered at $0$) of $f$; if $f(x)$ can be represented by a power series, then this is it (it's a unique representation).
- Q: Write the Taylor series representation of the following function and state the interval for which the representation converges: $$f(x) = \frac{1}{1-x}.$$ 
- A: This is a geometric series. We find $$\frac{1}{1-x}= 1 + x+x^2+x^3+\cdots = \sum_{n=0}^\infty x^n,$$ which is valid for $$-1 l< x < 1.$$
- Q: Write the Taylor series representation of the following function and state the interval for which the representation converges: $$f(x) = \frac{1}{1+x}.$$ 
- A: This is the geometric series with $-x$ substituted, $$\frac{1}{1+x}= 1 - x +x^2-x^3+\cdots = \sum_{n=0}^\infty (-1)^n x^n,$$ which is valid for $$-1 < x<1.$$
- Q: Write the Taylor series representation of the following function and state the interval for which the representation converges: $$f(x) = \log(1+x).$$ 
- A: This may be derived integrating the geometric series of $-x$: $$\int\frac{1}{1+x}dx = \log(1+x)= x -\frac{x^2}{2}+\frac{x^3}{3}-\cdots = \sum_{n=1}^\infty \frac{(-1)^n}{n}x^n,$$ (note the index begins at $1$). This series converges when $$-1< x\leq1.$$
- Q: Write the Taylor series representation of the following function and state the interval for which the representation converges: $$f(x) = e^x.$$ 
- A: Compute a few Taylor coefficients, then guess: $$e^x = 1 + x+\frac{x^2}{2!}+\frac{x^3}{3!}+\cdots = \sum_{n=0}^\infty\frac{1}{n!} x^n.$$ Turns out to be valid for all $x$ in $\RR$.
- Q: Write the Taylor series representation of the following function and state the interval for which the representation converges: $$f(x) = \sin x.$$ 
- A: Compute a few Taylor coefficients, then guess: $$\sin x = x+-\frac{x^3}{3!}+\frac{x^5}{5!}-\cdots = \sum_{n=0}^\infty\frac{(-1)^n}{(2n+1)!} x^{2n+1}.$$ Turns out to be valid for all $x$ in $\RR$.
- Q: Write the Taylor series representation of the following function and state the interval for which the representation converges: $$f(x) = \cos x.$$ 
- A: Compute a few Taylor coefficients, then guess:$$\cos x = 1+-\frac{x^2}{2!}+\frac{x^4}{4!}-\cdots = \sum_{n=0}^\infty\frac{(-1)^n}{(2n)!} x^{2n}.$$ Turns out to be valid for all $x$ in $\RR$.

## Leftovers

- Q: List $2^3$, $2^6$, $2^9$ and $2^{12}$ in decimal expansions. 
- A: We compute $8$, $64$, $512$ and $4092$ respectively.
- Q: List out $2^2$, $2^4$, $2^8$ and $2^{16}$ in decimal expansions. 
- A: We have $4$, $16$, $256$ and $65536$ respectively.
- Q: How do I use Lagrange multipliers to solve a constrained optimization problem? 
- A: Turn a calculus problem into linear algebra. Suppose we want $$\text{ min (or max) }f(x,y,z) \text{ subject to } g(x,y,z) =0,$$
    - Form the augmented function,$$L(x,y,z,\lambda) = f(x,y,z)-\lambda g(x,y,z)$$
    - Set all partial derivatives of $L$ equal to zero,
    - Solve for $x,y,z$.
- Q: What is the partial fraction decomposition of $$\frac{1}{(x-a)(x-b)}?$$ 
- A: This special case decomposes to the form $$\frac{1}{a-b}\left(\frac{1}{x-a}-\frac{1}{x-b}\right).$$
