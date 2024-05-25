---
layout: page
title: Dialogflow Migration
description: Enabling chatbot team transition from ES to CX
img: assets/img/dialogflow.jpg
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
**Tools**: Dialogflow Essentials (ES)/Customer Experience (CX), Miro, iMovie, OneNote <br>
**Timeline**: Q3 2021 

### Videos
I created multiple videos for the CD team explaining how to design in CX from scratch, ES versus CX differences, what the overall migration process would look like using established team tools/processes, and specific migration examples with their existing ES flows. 

I’ve included one of these videos below - it provides a high-level overview of CX concepts, and then builds out an example flow meant to help customers with DNS management.  


<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/sQcPesDUk9c" allowfullscreen=""></iframe>
</div>
<br>

### Reporting/Documentation

I generated additional reporting estimating how long the migration would take for existing major flows, with time estimates for building using both the existing CX custom payload templates versus a Chrome extension built by one of our developers. 

I also created documentation highlighting current pain points the team had with ES agents, and whether migrating to CX would solve the issue. I’ve included some of the more generalizable points in the table below. 

Areas I feel would generate the most time savings for designers are &#11088; starred. Green cells indicate that CX provides a complete solution, blue cells indicate that a partial solution is provided, and red cells indicate that a solution is not provided. 

_Note: There are some differences in vocabulary between ES/CX. For example, “intent” in ES encompasses training phrases, actions, parameters, and responses, while an intent in CX has been simplified into just training phrases and parameters, making them more reusable._

_Note: This table has not been updated to reflect platform changes since 2022._

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th scope="col" width="50%">ES Pain Point</th>
      <th scope="col" width="50%">Solved by CX?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Need to click to expand nested intents when designing </td>
      <td style="background-color: #77DD77">&#11088; Everything is automatically “expanded” due to the visual nature of CX - there is no need for clicking, all pages and their subsequent routes are displayed by default. This saves time when accessing intents. Additionally, not having nested intents makes searching for specific intents faster by allowing for easier filtering.</td>
    </tr>
    <tr>
      <td>If your team uses visual companions to represent flows, these need to be built manually in a separate platform</td>
      <td style="background-color: #77DD77">The CX console user experience for is visual graphs instead of mostly text forms, potentially replacing need for secondary visual companion</td>
    </tr>
    <tr>
      <td>Webhook responses must occur within 10 seconds for Google Assistant apps/within 5 seconds for all other apps, or request will time out </td>
      <td style="background-color: #77DD77">Can set custom webhook response timeouts</td>
    </tr>
    <tr>
      <td>Webhooks must be applied for the whole agent (they cannot be applied on individual intents). This may prevent use of webhooks even when some are desired.</td>
      <td style="background-color: #77DD77">Webhooks can be applied on individual intents</td>
    </tr>
    <tr>
      <td>ES only allows a single webhook to be defined for fulfillment</td>
      <td style="background-color: #77DD77">CX allows you to specify multiple fulfillment webhooks</td>
    </tr>
    <tr>
      <td>Test agent in ES console doesn’t showcase entirety of conversation, need to know triggers for whole flow or use OneNote/website test environment to keep track of test conversation</td>
      <td style="background-color: #77DD77">CX test agent can show entire conversation, includes additional features (e.g., replay, save test cases, toggle on/off sentiment analysis, webhooks, partial response)</td>
    </tr>
    <tr>
      <td>New/requested features will not continue to be supported on ES</td>
      <td style="background-color: #77DD77">New features and functions will be supported on CX</td>
    </tr>
    <tr>
      <td>Time spent entering similar batches of training phrases multiple times</td>
      <td style="background-color: #77DD77">&#11088; Intents now only include training phrases instead of responses as well, allowing for the same intent to be used in multiple cases</td>
    </tr>
    <tr>
      <td>Context issues: Steep initial learning curve, no comprehensive overview of where contexts “touch”</td>
      <td style="background-color: #A7C7E7">&#11088; CX does not use contexts, state handlers (routes/event handlers) are used to control conversational paths. Graphs show where pages connect - however, still need to click into state handlers to see which intents drive which pages.</td>
    </tr>
    <tr>
      <td>No built-in way to track changes, need to use external note-taking method (e.g. Excel), which can be time-consuming</td>
      <td style="background-color: #A7C7E7">“Change History” feature being built out, currently available as preview - however, probably still not as comprehensive/easy to reference as custom notes</td>
    </tr>
    <tr>
      <td>Need to export all content whenever publishing, potentially overriding content that is currently being worked on</td>
      <td style="background-color: #f1807e">No, the same issue remains. Additionally, in CX, the export would be in a proprietary file format that we wouldn’t be able to modify like we can with the zip files in ES. </td>
    </tr>
    <tr>
      <td>Need to use payloads for buttons/other rich responses, cannot see these in Dialogflow environment</td>
      <td style="background-color: #f1807e">No, the same issue remains</td>
    </tr>
  </tbody>
</table>

