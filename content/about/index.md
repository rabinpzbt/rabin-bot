---
layout: layouts/base.njk
eleventyNavigation:
  key: About Me
  order: 4
numberOfLatestPostsToShow: 2
---
{% set postsCount = collections.posts | length %}
{% set latestPostsCount = postsCount | min(numberOfLatestPostsToShow) %}
# About Me

I obtained my undergraduate degree in computer science during the first few weeks of the COVID-19 pandemic. Fast forward to today, I am currently enrolled in the Juris Doctor (J.D.) program of the University of Santo Tomas Faculty of Civil Law. 

When granted the luxury of free time, I scramble to finish my video game backlogs. While creativity has oftentimes evaded me, I try to write a paragraph or two to keep the "frustrated-writer-flame" burning. Other interests of mine include data analysis and hoarding, journalism, Pokémon, and politics.