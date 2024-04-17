---
layout: page
title: Dialogflow Migration
description: Enabling chatbot team transition from ES to CX
img: assets/img/7.jpg
importance: 3
category: work
toc:
  sidebar: left
---
## Problem
The [GoDaddy](https://www.godaddy.com/) Conversational Design (CD) team was evaluating whether they should transition from [Dialogflow Essentials](https://cloud.google.com/dialogflow/es/docs) (agent type used for the existing customer support bot), to [Dialogflow Customer Experience](https://cloud.google.com/dialogflow/cx/docs) (a newer, more advanced agent type). While CX supports much more complex conversations, the team had not explored it in depth, and was unsure of the pros and cons of transitioning their 400+ existing ES intents.

## Solution
Create tutorial videos demonstrating the basics of how to design conversational flows in CX, with examples using existing flows from the GoDaddy customer support bot. Generate documentation estimating potential lift of migrating all existing ES intents, comparing possible time savings moving forward. 

## Deliverables
<strong>Tools</strong>: Dialogflow Essentials (ES), Dialogflow Customer Experience (CX), Miro, iMovie, OneNote <br>
<strong>Timeline</strong>: Q3 2021 

### Videos
I created multiple videos for the CD team explaining how to design in CX from scratch, ES versus CX differences, what the overall migration process would look like using established team tools/processes, and specific migration examples with their existing ES flows. 

I’ve included one of these videos below - it provides a high-level overview of CX concepts, and then builds out an example flow meant to help customers with DNS management. 

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/sQcPesDUk9c" allowfullscreen></iframe>
</div>

### Reporting/Documentation

I generated additional reporting estimating how long the migration would take for existing major flows, with time estimates for building using both the existing CX custom payload templates versus a Chrome extension built by one of our developers. 

I also created documentation highlighting current pain points the team had with ES agents, and whether migrating to CX would solve the issue. I’ve included some of the more generalizable points in the table below. Areas I feel would generate the most time savings for designers are &#11088; starred. 

_Note: There are some differences in vocabulary between ES/CX. For example, “intent” in ES encompasses training phrases, actions, parameters, and responses, while an intent in CX has been simplified into just training phrases and parameters, making them more reusable._

_Note: This table has not been updated to reflect platform changes since 2022._


