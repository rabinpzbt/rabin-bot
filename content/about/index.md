---
layout: layouts/home_alt.njk
eleventyNavigation:
  key: About Me
  order: 4
numberOfLatestPostsToShow: 2
---
{% set postsCount = collections.posts | length %}
{% set latestPostsCount = postsCount | min(numberOfLatestPostsToShow) %}
# About Me 

I obtained my <strong class="aboutLinks"> undergraduate degree in computer science</strong> during the first few weeks of the COVID-19 pandemic. Fast forward to today, I am currently enrolled in the Juris Doctor (J.D.) program of the <strong class="aboutLinks"> University of Santo Tomas Faculty of Civil Law</strong>. From time to time, I engage in freelance front-end development. 

When granted the luxury of free time, I scramble to finish my video game backlogs. While creativity has oftentimes evaded me, I try to write a paragraph or two to keep the "frustrated-writer-flame" burning. Other interests of mine include data analysis and hoarding, journalism, Pokémon, and politics.
<!--
<div class="aboutContainer">
  <div class="rowContainer">
          <div class="columnContainer col-3">2022—present</div>
          <div class="columnContainer"> JD program, UST Faculty of Civil Law</div>
        </div>
        <div class="rowContainer">
        <div class="columnContainer">stuff</div>
    </div>    
</div>

<div class="aboutContainer">
  <div class="rowContainer">
          <div class="columnContainer col-3">2015—2020</div>
          <div class="columnContainer"> JD program, UST Faculty of Civil Law</div>
        </div>
        <div class="rowContainer">
        <div class="columnContainer">stuff</div>
    </div>    
</div>
    -->
