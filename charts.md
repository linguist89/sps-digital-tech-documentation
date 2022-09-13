---
layout: page
title: Charts
navigation: 3
---

# Adding a chart
Charts have two properties which are needed to create them `chart_info` and `chart_build_details`. The easiest way to add them to a form is via the client code, so that you can customize their heights and add them to a flow panel grid. The form name is `GenericChart` and they have been designed to be able to use them without other dependencies.

## Chart_info
`chart_info` is a dictionary that must contain the following data:


 - `chart_number` - this is used when the chart is created to make sure that the chart has a unique id, so that it doesn't conflict with other charts being created. The charts' ids take the form `generic-chart` + chart_number.
 - `labels` - this is a list if `str` that will be the labels of the x-axis of the chart.
 - `data` - this is a list of `int` or `float` which be the x-axis data.

 Examples of adding these are available with all templates that have charts on them as well as databases that contain synthetic data to illustrate the type of data required.

## Chart_build_details

In `MainModule` there is a function called `get_chart_build_details` which takes as a parameter the `chart_info` and returns the `chart_build_details` variable. This variable is consistent with the dictionary syntax that is needed to create the chart in Javascript, so there isn't a need to change this unless you want to customize the charts, but then you would need to know how the Javascript syntax works.
