---
layout: splash
title: Overview
permalink: /
description: Introduction of this project

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

<div class=".l-page">
  {% include figure.liquid path="assets/img/leaf.jpg" title="leafs" class="img-fluid rounded z-depth-1" %}
</div>

Hi, this blog is a comprehensive guide to build the components for a plant irrigation system using a diy capacitive soil moisture sensor. I would be happy, if these pages here inspire and help people to build their own version for their plants at home, garden or even a field. I'll focus on my plants at home, as I don't have access to a garden and it's also making my live a lot easier to use an environment that is in my reach and control. I tried to realize this project with rather cheap and easily available components. My aim was to get something reliable and affordable done that waters around ten different plants independently. Depending on the use-case and a more careful selection of the needed parts one could probably reduce the price even more to only a few euros or dollars.

My name is Mario. I am actually a software engineer spending my entire work life in automotive industry building car navigation systems and in recent years creating LiDAR perception software. 

But the question who waters my plants when I am not at home and pure curiosity in the details of how soil moisture can be measured let me start this project which is more related to electronics. 

The structure of this blog will be:
 
 * Motivation and related work
   * Types of sensors and their costs
   * Available Sensors
   * Theory of capacitive sensors
   * Frequency/Soil/Temperature/Salt dependency
   * Advantages/Disadvantages
   * Related Work and Papers
 * Building and testing prototypes
   * Frequency counting vs Peak detector
   * Circuits
   * Frequency Generator
 * Building a 20 MHz capacitive soil moisture sensor
   * Parts / Price
   * Structure / 
   * Calibration
   * Seal / Water Proof
 * Building a 120 MHz capacitive soil moisture sensor
   * Parts / Price
   * Frequency Generator Circuit
   * Warning
   * Structure  
   * Calibration   
 * Evaluating the differences of a 20 MHz and a 120 MHz soil moisture sensor
 * Connecting a Pump
 * Online Data and Remote Control
 * Possible Applications and Further Development 

{% assign sorted_projects = site.projects | sort: "importance" %}

<!-- Generate cards for each project -->
<div class="container">
  <div class="row row-cols-2">
  {% for project in sorted_projects %}
    {% include projects_horizontal.liquid %}
  {% endfor %}
  </div>
</div>
