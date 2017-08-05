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

or it can be written as :

$$ \frac{-y}{\sqrt{1 + y^2}}dy = \frac{\sqrt{1+ x^2}}{x}dx$$

We have reduced the original differential equation into a variable separable equation and it can be easily solved by integrating both sides.  

$$\int \frac{-y}{\sqrt{1 + y^2}}dy = \int \frac{\sqrt{1+ x^2}}{x}dx$$

As we are using indefinite integral , so we need to introduce an arbitrary constant but for smooth calculations ,I'll introduce it directly in my answer.

<b>Solving LHS integral:</b>

$$\int \frac{-y}{\sqrt{1 + y^2}}dy.     \cdots  eq(1)$$     

assuming $1+y^2 = t$ then we'll have $$2y dy = dt \\  ydy = \frac{dt}{2}$$ <br />
putting value of $ydy$ into equation (1) ,we have

$$ =\int \frac{-dt}{2 \sqrt{t}}
$$

$$ =\frac{-1}{2} \int t^{-1/2} dt$$

$$=  - t^{1/2} $$ 

$$=  \sqrt{t} $$

Replacing $t$ by $1+y^2$ , we have

$$= - \sqrt{1+y^2}$$

<b>Solving RHS integral :</b> 

$$= \int \frac{\sqrt{1+ x^2}}{x}dx  \cdots eq(2)$$

Let $\sqrt{1+x^2} = u $ then $$ \frac{x}{\sqrt{1+x^2}}dx = du , \\ dx = \frac{\sqrt{1+x^2}}{x}du $$ <br />
putting values of $dx$ and $u$ into equation (2) we have

$$= \int \frac{u^2}{u^2 -1}du \\ =\int (1+ \frac{1}{u^2 -1}) du \\ = u + \int \frac{1}{(u-1)(u+1)}du \\= u + \int \frac{1}{2}\left[\frac{1}{u-1}-\frac{1}{u+1}\right]du \\= u + \frac{1}{2}\left[\ln\left|(u-1)\right|-\ln\left|(u+1)\right| \right] \\= u + \frac{1}{2} \ln\left(\left|\frac{u-1}{u+1}\right|\right)$$

Replacing $u$ by $\sqrt{x^2 +1}$, we have

$$= \sqrt{x^2 +1} + \frac{1}{2} \ln\left(\left|\frac{\sqrt{x^2 +1}-1}{\sqrt{x^2 +1}+1}\right|\right)$$

Hence , our solution to differential equation is :

$$C - \sqrt{1+y^2} = \sqrt{x^2 +1} + \frac{1}{2} \ln\left(\left|\frac{\sqrt{x^2 +1}-1}{\sqrt{x^2 +1}+1}\right|\right)$$

where $C$ is arbitrary constant.

<div class="box1">
<p>
<b>Answer 1</b><br />

$$\sqrt{x^2 +1} +\sqrt{y^2 +1} + \frac{1}{2} \ln\left(\left|\frac{\sqrt{x^2 +1}-1}{\sqrt{x^2 +1}+1}\right|\right) = C $$

where $C$ is arbitrary constant.

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

where $C$ is arbitrary constant.






<hr />
## Solution 3
Given Differential equation is :

$$(x^3 + y^3)dx - (x^2 y + x y^2)dy =0$$

or it can be written as 

$$ \frac{dy}{dx} = \frac{(x^3 + y^3)}{(x^2 y + x y^2)} $$

This is homogeneous differential equational and it can be easily solved by substituting 
$$y = vx$$ then <br />
$$\frac{dy}{dx} = v + x \frac{dv}{dx}$$ <br />
Putting values of $y$ and $\frac{dy}{dx}$ , we get

$$ v + x \frac{dv}{dx} = \frac{x^3 + (vx)^{3}}{x^2 (vx) + x (vx)^{2}} \\ = \frac{x^3 (1+ v^{3})}{x^3 ( v+ v^2)} \\ = \frac{1+ v^{3}}{ v+ v^2}$$

$$ x \frac{dv}{dx} = \frac{1+ v^{3}}{ v+ v^2} -v \\= \frac{1+ v^3 - v^2 -v^3}{ v+ v^2} \\=  \frac{1 - v^2}{ v+ v^2}$$

or it can be written as


$$\frac{v + v^2}{1- v^2}dv = \frac{dx}{x}$$

Clearly, it is a variable separable form , so it can be solved by integrating both sides.

$$\int \frac{v + v^2}{1- v^2}dv = \int \frac{dx}{x}$$

$$\int \frac{(v+1) + (v^2 -1)}{1- v^2}dv = \int \frac{dx}{x}$$

<center>Applying linearity:
</center>

$$\ln|x|+ C = \int \left[\frac{v+1}{1- v^2} +\frac{v^2 -1}{1- v^2} \right]dv$$

$$ = \int \left[\frac{v+1}{(v+1)(1-v)} +\frac{-(1-v^2)}{1- v^2} \right]dv$$

$$ \ln|x| + C= -\ln|1-v| - v $$


As we have earlier substuited $y=vx$ , that means $v =\frac{y}{x}$..substituting value of $v$ in above equation. 


$$ \ln|x| + C= -\ln\left|1-\frac{y}{x}\right| - \frac{y}{x} $$


$$C+ \ln|x| +\ln\left|\frac{x-y}{x}\right| + \frac{y}{x} = 0$$

Using properties of log function , $\ln(a)+ \ln(b) = \ln(ab)$

$$ \ln|x-y| + \frac{y}{x} + C=0$$

Hence , our final answer is :
<div class="box1">
<p>
<b>Answer 3</b><br />

$$ \ln|x-y| + \frac{y}{x} + C=0$$

where $C$ is arbitrary constant.

</p>
</div>


<hr />
## Solution 4
Given Differential equation is :

$$(3y-7x+7)dx + (7y-3x+3)dy = 0$$

or it can be written as 

$$ \frac{dy}{dx} = \frac{-3y+7x-7}{7y-3x+3} \\ = \frac{-3y+7(x-1)}{7y-3(x-1)}$$

Let us assume $x-1 =t$ , then$ dx = dt$ ,putting these in above equation. We have,

$$ \frac{dy}{dt} = \frac{-3y+7t}{7y-3t}$$

Clearly,This is an homogenous differential equation and it can be easily solved by substituting $y= vt$ \then $\frac{dy}{dt} = v + t \frac{dv}{dt}$.

$$\therefore  v + t \frac{dv}{dt} = \frac{-3(vt)+7t}{7(vt)-3t} \\ = \frac{-3v+7}{7v-3} \\ \iff t \frac{dv}{dt} =\left(\frac{-3v+7}{7v-3}\right)-v \\ =\frac{-3v+7-7v^2+3v}{7v-3} \\ =\frac{7(1-v^2)}{7v-3}$$

Or it can be written as

$$\frac{dt}{t} =\left[\frac{7v-3}{7(1-v^2)}\right]dv$$

It is now changed into variable separable form and it is solved by integrating both sides.

$$\int \frac{dt}{t} =\int \left[\frac{7v-3}{7(1-v^2)}\right]dv$$

<center>Applying linearity</center>

$$\ln|Ct| =\int \left[\frac{7v}{7(1-v^2)}\right]dv - \int \left[\frac{3}{7(1-v^2)}\right]dv$$

<p align="right">where $C$ is arbitrary integration constant.</p>

$$\ln|Ct| = \int \frac{1}{-2}\left[\frac{-2v}{1-v^2}\right]dv - \int \frac{3}{7}\left[\frac{1}{1-v^2}\right]dv$$

$$\ln|Ct| =  \frac{-1}{2}\left[\ln|1-v^2|\right] -\frac{3}{14}\ln\left|\frac{v+1}{v-1}\right|$$

Putting $v= \frac{y}{t}$
 
$$\ln|Ct| =  \frac{-1}{2}\left[\ln|1-{\frac{y}{t}}^2|\right] -\frac{3}{14}\ln\left|\frac{\frac{y}{t}+1}{\frac{y}{t}-1}\right|$$

$$\ln|Ct| =  \frac{-1}{2}\left[\ln|\frac{t^2 - y^2}{t^2}|\right] -\frac{3}{14}\ln\left|\frac{y+t}{y-t}\right|$$

Putting $t =x-1$ , We have 

$$\ln|x-1| + \lnC =  \frac{-1}{2}\left[\ln|\frac{(x-1)^2 - y^2}{(x-1)^2}|\right] -\frac{3}{14}\ln\left|\frac{y+x-1}{y-x+1}\right|$$

<div class="box1">
<p>Solution : <br />
$$\ln|x-1| + \lnC =  \frac{-1}{2}\left[\ln|\frac{(x-1)^2 - y^2}{(x-1)^2}|\right] -\frac{3}{14}\ln\left|\frac{y+x-1}{y-x+1}\right|$$
</p>
</div>

<hr />
## Solution 5
Given Differential equation is :
![page-1-solution-question-5](//sirkapil.github.io/alpha/img/5-1.jpg)
<hr />
## Solution 6
Given Differential equation is :

<hr />
## Solution 7
Given Differential equation is :
![page-1-solution-question-7](//sirkapil.github.io/alpha/img/7-1.jpg)<br />

![page-2-solution-question-7](//sirkapil.github.io/alpha/img/7-2.jpg)<br />

![page-3-solution-question-7](//sirkapil.github.io/alpha/img/7-3.jpg)
<hr />
## Solution 8
Given Differential equation is :
![page-1-solution-question-8](//sirkapil.github.io/alpha/img/8-1.jpg)<br />

![page-2-solution-question-8](//sirkapil.github.io/alpha/img/8-2.jpg)<br />
<hr />
## Solutiyon 9
Given Differential equation is :
![page-1-solution-question-9](//sirkapil.github.io/alpha/img/9-1.jpg)<br />

![page-2-solution-question-9](//sirkapil.github.io/alpha/img/9-2.jpg)
<hr />
## Solution 10
Given Differential equation is :

