---
---

<!-- # Nice to Meet You! -->

<!--<img align="left" width="300" height="400" src="images/Tianyi_portrait.HEIC">-->

{% capture text %}

My name is Tianyi Liu, currently a fifth year Ph.D. student in the [Department of Biostatistics](https://sph.unc.edu/bios/biostatistics/) at The University of North Carolina Gillings School of Global Public Health and a Triple Tar Heel candidate. My research is related to cell-type deconvolution and precision medicine. I also like to work with a diverse set of collaborators and use my expertise in statistical modeling and machine learning to solve prblems in public health and big data. You can find my publications and projects on this website.

In my spare time, I like to read, hike, travel, go to gym, play soccer or basketball, try new board games, and play hold'em poker. My favorite sport is soccer. I also enjoy spending time with my friends and my cat [Wrigley](members/wrigley.html).

{%
  include button.html
  link="members/tianyi-liu.html"
  text="Read my full bio"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}


{%
  include feature.html
  image="images/headshot.jpg"
  link="members/tianyi-liu.html"
  title="About Me"
  text=text
%}


<!-- {%
  include portrait.html
  lookup="tianyi-liu"
  style="small"
%} -->

<!-- <div align="center">
  <img width=480 src="images/Tianyi_portrait.HEIC">
</div> -->

<!-- {% capture lorem %}
_Lorem_ **ipsum**.
{% endcapture %}

{%
  include alert.html
  type="info"
  content=lorem
%} -->


{% include section.html %}

## Highlights

{% capture text %}

My independent research spans questions regarding cell-type deconvolution, relying heavily on theories and algorithms of matrix factorization. I also dab in collaboration in precision medicine, work with a group of scientists on quantifying genetic impacts of inorganic arsenics on type-II diabetes using mouse models, and consult on statistical analysis for neonatal physical therapeutic interventions.

{%
  include button.html
  link="research"
  text="See my publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="My Research"
  text=text
%}

{% capture text %}

My Highlighted projects include a collaboration with UNC Women's Soccer, an R package for cell-type deconvolution named ARTdeConv.

{%
  include button.html
  link="projects"
  text="Browse my projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="projects"
  title="My Projects"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

You can also follow some of my close colleagues and friends. See what they are up to these days!

{%
  include button.html
  link="team"
  text="Meet my colleagues and friends"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="team"
  title="Colleagues & Friends"
  text=text
%}

{% include section.html %}

## Blog Posts

Here are some of my highlighted blog posts:

{%
  include post-excerpt.html
  lookup="example-post-1"
%}
