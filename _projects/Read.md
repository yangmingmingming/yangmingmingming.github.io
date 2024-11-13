---
name: Vega Lite HW6
tools: [Python, HTML, vega-lite]
image: assets/pngs/visualization3.pngs
description: This is a "showcase" project that uses vega-lite for HW6!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Visual
Use following 

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/combine.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/combine.json" style="width: 100%"></vegachart>




## Explanation
Pic1
-This scatter plot visualizes the relationship between the Square Footage of properties and the Year Acquired. The color encodes the number of Floors Above Grade, binned into distinct categories.

-Encoding Types:
X-axis: Square Footage 
Y-axis: The log scale for the y-axis ("Year Acquired")  adjust the data distribution
Color: Represents Floors Above Grade (ordinal variable).

-The Data Transformations I have been working with is Binning(The Floors Above Grade variable was binned into several ranges to simplify visualization.) 

-The Interactivity tool(Brush and selection parameters are added to the plot for filtering and highlighting data dynamically) help me display property-specific details .

Pic2
-This scatter plot displays the relationship between Square Footage and Rep Dist. which  helps identify trends in property sizes across various districts over specified time ranges.

-X-axis: Encodes Square Footage as a quantitative variable to represent property size. Y-axis: Rep Dist (ordinal scale) to display categorical groupings.

-Data Transformation: The temporal variable "Year Acquired" was transformed to a log 

-Interactivity: Brush and dropdown filters enhance interactivity by dynamically updating plots based on selected counties

Pic3
The third visualization combines the first two plots, offering a side-by-side comparison of the relationship between Square Footage and both Year Acquired and Rep Dist, with distinct color encodings for Floors Above Grade and Congress Dist. Interactive elements, including a dropdown filter for county selection and brushing to highlight related points across plots, enhance data exploration and engagement. This integrated view allows users to simultaneously identify patterns in property size, acquisition trends, and district-specific variations, making the analysis more comprehensive and accessible.


## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

