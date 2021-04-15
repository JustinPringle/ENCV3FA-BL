---
title: Head Loss
teaching: 0
exercises: 25
questions:
  - "Can you develop approporiate dimensionless groups to describe the flow of water in a pipe?  "
objectives:
- Use the method of Scales to form Pi groups
- develop \\(\\Pi\\) groups for pipe flow
keypoints: 
- The number of base dimensions was 3.
- The number of variables was 7.
- We could form 4 \\(\\Pi\\) groups.
- with a bit of interpretation we found \\(h_f\\) as the Darcy-Weisbach equation
---

# The Problem
The change in pressure along a pipe \\(\Delta P\\) is assumed to depend on the following quantities:
- Fluid density \\(\rho\\),
- Fluid viscocity \\(\mu\\),
- Flow velocity \\(U\\),
- The pipe diameter \\(D\\),
- The pipe length \\(l\\),
- and the roughness of the pipe \\(\epsilon\\),

\\[\Delta P = \mathcal{F}(U,D,l,\epsilon,\rho,\mu)\\]
Can you construct dimensionless groups that describe pipe flow?

>## Challenge
> How many \\(\\Pi\\) groups can be formed?
> > ## Solution
> > - The number of dimensions is 3 i.e. \\(m = 3\\)
> > - the number of variables is 7 i.e. \\(n=7\\)
> > - Therefore \\(n-m=4\\)
> {: .solution}
{: .challenge}

### Now What?
It's good practise to write out the units of the problem variables in terms of their dimensions:

\\(
  \\begin{align}
  [P] &= ML^{-1}T^{-2} \newline
  [U] &= LT^{-1} \newline
  [\epsilon] = [l] = [D] &= L \newline
  [\rho] &= ML^{-3} \newline
  [\mu] &= ML^{-1}T^{-1}
  \\end{align}
\\)

So now we have our units i.t.o their basic dimensions as well as the number of dimensionless groups that we can form so... let's do it!

Our base dimensions are:
- length \\(L\\),
- Mass \\(M\\),
- Time \\(T\\)

Select \\(\rho\\), \\(U\\) and \\(D\\) as scaling parameters:

Let's derive the first scaling dimension together and then you try on your own to solve the rest:

>
>Let's construct the time scale:
>
>if we use \\(\\rho\\), \\(U\\) and \\(D\\) as scaling variables, then for time \\
> \\(T\\rightarrow \\frac{D}{U}\\)
{: .challenge}

>## Challenge
>What are the remaining dimensions in terms of the scaling parameters?
> > ## Answer
> > \\(L \\to D\\) \\
> > \\(M \\to \\rho D^3\\)
>{: .solution}
{: .challenge}

## Non-Dimensionalize

>## Challenge
> What are the \\(\Pi\\) terms?
> > ## Answer
> > \\[\frac{\Delta P}{\rho U^2} = \mathcal{F_1}\left(\frac{UD\rho}{\mu},\frac{l}{D},\frac{\epsilon}{D}\right)\\]
>{: .solution}
{: .challenge} 

## Interpret

How do we interpret this result?

If we assume that \\(\frac{\Delta P}{\rho U^2} \propto \frac{l}{D}\\), and this seems reasonable then we could rewrite the above function as

\\[\Delta P= \rho U^2\frac{l}{D}\mathcal{F_1}\left(\frac{UD\rho}{\mu},\frac{\epsilon}{D}\right)\\]

>## Challenge
> what is \\(\frac{UD\rho}{\mu}\\)?
>> ## answer
>> \\(Re\\), the Reynolds number
> {: .solution}
{: .challenge}

now if \\(h_f = \frac{\Delta P}{\rho g}\\), what is \\(\mathcal{F_1}\left(\frac{UD\rho}{\mu},\frac{\epsilon}{D}\right)\\)?

> ## answer
> The friction factor
 {: .solution}

 Putting this all together and scaling by a factor of 2 from experimental data:

 \\[h_f = f\frac{l}{D}\frac{U^2}{2g}\\]