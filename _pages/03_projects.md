---
layout: page
title: projects
permalink: /projects/
description: Some of my previous projects
order: 4
---
<pre> 
                 Applied Machine Learning (Vision and NLP)
</pre>

{% for project in site.ml_projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}" />
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        {% else %}
        <!-- <div class="thumbnail blankbox"></div> -->
           <br /> 
       {% endif %}    

        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
         <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="center" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}" style="height:100%; width:100%"/>
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        {% else %}
        <!--<div class="thumbnail blankbox"></div>  -->
               <br />
        {% endif %}    

        </a>
    </div>
</div>


{% endif %}

{% endfor %}

<pre> 
                    Data Analytics and Engineering
</pre>
{% for project in site.data_projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}" style="height:100%; width:100%"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}

