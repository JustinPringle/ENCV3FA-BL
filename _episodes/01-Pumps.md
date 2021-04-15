---
title: Pumps
teaching: 0
exercises: 25
questions:
  - "Can you develop approporiate dimensionless groups to describe the flow of water through a pump?  "
objectives:
- Use the method of Scales to form Pi groups
- develop \\(\\Pi\\) groups for pipe flow through pumps
keypoints: 
- The number of base dimensions was 3.
- The number of variables was 7.
- We could form 4 \\(\\Pi\\) groups.
- with a bit of interpretation we found \\(h_f\\) as the Darcy-Weisbach equation
---

# The Problem
The change in pressure through a pump \\(\Delta P\\) is assumed to depend on the following quantities:
- Fluid density \\(\rho\\),
- Flow rate \\(Q\\),
- The pipe diameter \\(D\\),
- and the rotational speed \\(N\\),

\\[\Delta P = \mathcal{F}(D,Q,\rho,N)\\]
Can you construct dimensionless groups that describe pipe flow?

>## Challenge
> How many \\(\\Pi\\) groups can be formed?
> > ## Solution
> > - The number of dimensions is 3 i.e. \\(m = 3\\)
> > - the number of variables is 5 i.e. \\(n=5\\)
> > - Therefore \\(n-m=2\\)
> {: .solution}
{: .challenge}

>## Advanced Challenge
> Why is viscosity neglected?
> > ## Answer
> > Flow through a pump is turbulent and therefore the effect of viscosity is neglegible (i.e. the Reynolds number is large)
>{:.solution}
{:.challenge}

### Units
It's good practise to write out the units of the problem variables in terms of their dimensions:

\\(
  \\begin{align}
  [P] &= ML^{-1}T^{-2} \newline
  [U] &= LT^{-1} \newline
  [\rho] &= ML^{-3} \newline
  [Q] &= L^3T \newline
  [N] &= T^{-1}
  \\end{align}
\\)

So now we have our units i.t.o their basic dimensions as well as the number of dimensionless groups that we can form so... let's do it!

Our base dimensions are:
- length \\(L\\),
- Mass \\(M\\),
- Time \\(T\\)

Select \\(\rho\\), \\(N\\) and \\(D\\) as scaling parameters:

Let's derive the first scaling dimension together and then you try on your own to solve the rest:

>
>Let's construct the time scale:
>
>if we use \\(\\rho\\), \\(D\\) and \\(N\\) as scaling variables, then for time \\
> \\(T\\rightarrow N^{-1}\\)
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
> > \\[\frac{\Delta P}{2 \rho D^2 N^2} = \mathcal{F_1}\left(\frac{Q}{D^3N}\right)\\]
>{: .solution}
{: .challenge} 

## Interpret

How do we interpret this result?

Assuming the pumps are geometric similar (the sizes are related) and Reynolds number effects are small we can generate **ONE** curve for all pump sizes!

Check it out for yourself (you will need to convert Pressure to head):

- Convert the pump curve below for various rpm (\\(N\\)), flow (\\(Q\\)) and head (hint: \\(h=\frac{P}{\rho g}\\)). 
- plot the data using you non-dimensionless terms and you should see the data collapse.

download the pdf [here]({{page.repository}})
<!-- "../data/pumps/Umzimkulu - Extraction - Submersibles - Dry-prime option.pdf"){:target="_blank"} -->
