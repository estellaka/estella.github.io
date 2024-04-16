---
layout: page
title: FullStory Documentation
description: Onboarding materials for the the GoDaddy Digital Care organization
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
toc:
  sidebar: left
---
### Problem
The [GoDaddy](https://www.godaddy.com/) Digital Care (DC) organization had been provided with licenses for [FullStory](https://www.fullstory.com/) (a behavioral data analytics tool), but there was minimal team adoption due to a lack of knowledge around how to use the tool and its potential value.

### Solution
I created a documentation library and held both team and individual workshops onboarding the DC writing and video teams (~20 members) to the platform.  

### Deliverables

#### Tools
FullStory, Confluence, Jira

#### Documentation
I created a Confluence library of documentation that included longer-form onboarding content, as well as shorter task articles targeted at filling gaps in team data that our current tools (e.g. Tableau Dashboards) cannot provide insight into. 

I’ve recreated some of the more generalizable documentation pieces below, as they may be useful for other FullStory users. They’ve been edited to remove confidential information, but the webpages used in examples are primarily from the [GoDaddy Help Center](https://www.godaddy.com/help)GoDaddy Help Center (our customer facing knowledge base). 

- <strong>FullStory "Crash Course"</strong>: This is a short onboarding document summarizing the core functionalities of the FullStory platform. 

- <strong>FullStory Tutorial - Tracking User Journeys</strong>: This article compares three built-in ways the FullStory platform provides to track user movement on websites, and proposes an alternative metric that can be built to track source traffic. 

#### Workshops

Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: Onboarding the GoDaddy Digital Care organization onto the FullStory platform
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
