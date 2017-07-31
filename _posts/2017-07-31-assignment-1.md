---
layout: post
title: Assignment 1
author: Kapil Chaudhary
---
![Assignment - questions](//sirkapil.github.io/alpha/img/assignment1.jpg)

## Solution 1
Given Differential equation is :

$$ \sqrt{(1+ x^2 + y^2 + x^2 y^2)} dx + (x y) dy = 0 $$

taking $y^2$ common from $y^2 + x^2 y^2$.

$$ \sqrt{(1+ x^2) + y^2(1 + x^2)} dx + (xy) dy = 0 $$

taking $1+x^2$ common from $(1+ x^2) + y^2(1 + x^2)$

$$ \sqrt{(1+ x^2) (1 + y^2)} dx + (x y) dy = 0 $$

$$= \sqrt{1+ x^2} \sqrt{1 + y^2} dx + (x y) dy = 0 $$

or it can be written as

$$-(x y) dy = \sqrt{1+ x^2} \sqrt{1 + y^2} dx$$

or it can be written as

$$ \frac{-y}{\sqrt{1 + y^2}}dy = \frac{\sqrt{1+ x^2}}{x}dx$$

We have reduced the original differential equation into a variable separable equation and it can be easily solved by integrating both sides.  

$$\int \frac{-y}{\sqrt{1 + y^2}}dy = \int \frac{\sqrt{1+ x^2}}{x}dx$$

As we are using indefinite integral , so we need to introduce an arbitrary constant but for smooth calculations ,I'll introduce it directly in my answer.

<b>Solving LHS integral:</b>

$$\int \frac{-y}{\sqrt{1 + y^2}}dy.     \cdots  eq(1)$$     

assuming $1+y^2 = t$ then we'll have $$2y dy = dt \\  ydy = \frac{dt}{2}$$
putting value of $ydy$ into equation (1) ,we have

$$ =\int \frac{-dt}{\sqrt{t}} \\ =\int -t^{-1/2} dt \\ =  -\frac{t^{1/2}}{\frac{1}{2}} \\ = -2 \sqrt{t} $$

Replacing $t$ by $1+y^2$ , we have

$$= -2 \sqrt{1+y^2}$$

<b>Solving RHS integral :</b> 

$$= \int \frac{\sqrt{1+ x^2}}{x}dx  \cdots eq(2)$$

Let $\sqrt{1+x^2} = u $ then $$ \frac{x}{\sqrt{1+x^2}}dx = du , \\ dx = \frac{\sqrt{1+x^2}}{x}du $$ 
putting values of $dx$ and $u$ into equation (2) we have

$$= \int \frac{u^2}{u^2 -1}du \\ =\int (1+ \frac{1}{u^2 -1}) du \\ = u + \int \frac{1}{(u-1)(u+1)}du \\= u + \int \frac{1}{2}\left[\frac{1}{u-1}-\frac{1}{u+1}\right]du \\= u + \frac{1}{2}\left[\ln(u-1)-\ln(u+1) \right] \\= u + \frac{1}{2} \ln\left(\frac{u-1}{u+1} \right)$$

Replacing $u$ by $\sqrt{x^2 +1}$, we have

$$= \sqrt{x^2 +1} + \frac{1}{2} \ln\left(\frac{\sqrt{x^2 +1}-1}{\sqrt{x^2 +1}+1} \right)$$

Hence , our solution to differential equation is :

$$C -2 \sqrt{1+y^2} = \sqrt{x^2 +1} + \frac{1}{2} \ln\left(\frac{\sqrt{x^2 +1}-1}{\sqrt{x^2 +1}+1} \right)$$

where C is arbitrary constant.

<div class="box1">
<p>
<b>Answer 1</b><br />

$$2 \sqrt{1+y^2} + \sqrt{x^2 +1} + \frac{1}{2} \ln\left(\frac{\sqrt{x^2 +1}-1}{\sqrt{x^2 +1}+1} \right) = C $$

where C is arbitrary constant.

</p>
</div>


<hr />

## Solution 2
Given Differential equation is :

$$\frac{dy}{dx} = sin(x+2y) + cos(x+2y)$$

Substituting $x +2y = u$ , we have $$1 + 2\frac{dy}{dx} =\frac{du}{dx} \\ \frac{dy}{dx} = \frac{1}{2}\left[\frac{du}{dx}-1 \right]$$

After substituting values of $x+2y$ and  $\frac{dy}{dx}$, We have

$$ \frac{1}{2}\left[\frac{du}{dx}-1 \right] = sin(u) + cos(u)$$

$$ \frac{du}{dx}-1 = 2\left[sin(u) +cos(u)\right] \\ \frac{du}{dx} = 2sin(u) +2cos(u)+1 \\ \frac{du}{2sin(u) +2cos(u)+1} = dx$$

We have transformed the differentia equation into _variable separable form_, it can be easily solved by integrating both sides.

$$ \int \frac{1}{2sin(u) +2cos(u)+1}du = \int dx \\ \int \frac{1}{2sin(u) +2cos(u)+1}du = x + C$$

where C is arbitrary constant.






<hr />
## Solution 3
Given Differential equation is :

<hr />
## Solution 4
Given Differential equation is :

<hr />
## Solution 5
Given Differential equation is :

<hr />
## Solution 6
Given Differential equation is :

<hr />
## Solution 7
Given Differential equation is :

<hr />
## Solution 8
Given Differential equation is :

<hr />
## Solutiyon 9
Given Differential equation is :

<hr />
## Solution 10
Given Differential equation is :

