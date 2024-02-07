@def title = "Franklin Sandbox"
@def hasmath = true
@def hascode = true
 

# Set up

## Update title

## Update config.md file

* change author

* add site name for GitHub

## Create a table of contents

\toc

## Upload using GitHub Deskstop

# Examples

## How to enter text

"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."

Section 1.10.32 of "de Finibus Bonorum et Malorum", written by Cicero in 45 BC

"Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?"


## How to render math equations

$$ a^2 + b^2 = c^2 $$

$$ \frac{d}{dx} \int_a^x f(t)dt = f(x) $$

$$ \bar{x} = \frac{1}{n} \Big(\sum_{i=1}^n x_i \Big) = \frac{x_1 + x_2 + \cdots + x_n}{n}$$

$$
    \begin{alignedat}{3}
        2&x + y \space- &z &= &8 \\
        -3&x -y + 2&z &= \space&-11 \\
        -2&x + y + 2&z &= &-3
    \end{alignedat}
$$

$$
    M =
        \begin{bmatrix}
            \begin{aligned}
                &2 & &1 & -&1\space \\
                \space-&3 & -&1 & &2 \\
                -&2 & &1 & &2
            \end{aligned}
        \end{bmatrix} 
$$

## How to insert Julia code (with outputs)

Hello, World!

```julia:./ex11
println("Hello, World")
```

\show{./ex11}

Basic Math

```julia:./ex12
1 + 1
```

\show{./ex12}

Create a Function 

```julia:./ex13
function add(x, y)
    x + y
end
```

\show{./ex13}

Call Function

```julia:./ex14
add(2, 3)
```

\show{./ex14}

Random Numbers

```julia:./ex15
rand(5, 5)
```

\show{./ex15}

Using Libraries

```julia:./ex1
using LinearAlgebra, Random
Random.seed!(135)
a, b = randn(50), randn(50)
println(dot(a, b))
println(sum(ai * bi for (ai, bi) ∈ zip(a, b)))
```

\output{./ex1}

(yet another example that floating point arithmetics can be complicated).

$$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$

\newcommand{\E}{\mathbb E}

Surely some people remember the ordering, but I always forget:

$$ \varphi(\E[X]) \le \E[\varphi(X)] $$

for $\varphi$ convex.


## How to insert a table from a CSV file

## How to insert an image file

## How to insert a clickeable thumbnail to a YouTube video

## How to inject raw HTML

<!-- # Franklin syntax sandbox

This page is meant as a sandbox for Franklin Syntax so that you can quickly practice or experience things.

## Sandbox

Write whatever you want here to practice Franklin Syntax:

```julia:./ex1
using LinearAlgebra, Random
Random.seed!(135)
a, b = randn(50), randn(50)
println(dot(a, b))
println(sum(ai * bi for (ai, bi) ∈ zip(a, b)))
```

\output{./ex1}

(yet another example that floating point arithmetics can be complicated).

$$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$

\newcommand{\E}{\mathbb E}

Surely some people remember the ordering, but I always forget:

$$ \varphi(\E[X]) \le \E[\varphi(X)] $$

for $\varphi$ convex. -->
