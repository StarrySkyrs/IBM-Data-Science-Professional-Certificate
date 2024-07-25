# 8. Data Visualization with Python
## Summary: Introduction to Data Visualization Tools
- Data visualization is the process of presenting data in a visual format, such as charts, graphs, and maps, to help people understand and analyze data easily.

- Data visualization has diverse use cases, such as in business, science, healthcare, and finance.

- It is important to follow best practices, such as selecting appropriate visualizations for the data being presented, choosing colors and fonts that are easy to read and interpret, and minimizing clutter.

- There are various types of plots commonly used in data visualization.

  - Line plots capture trends and changes over time, allowing us to see patterns and fluctuations.

  - Bar plots compare categories or groups, providing a visual comparison of their values.

  - Scatter plots explore relationships between variables, helping us identify correlations or trends.

  - Box plots display the distribution of data, showcasing the median, quartiles, and outliers.

  - Histograms illustrate the distribution of data within specific intervals, allowing us to understand its shape and concentration.

- Matplotlib is a plotting library that offers a wide range of plotting capabilities.

- Pandas is a plotting library that provides Integrated plotting functionalities for data analysis.

- Seaborn is a specialized library for statistical visualizations, offering attractive default aesthetics and color palettes.

- Folium is a Python library that allows you to create interactive and customizable maps.

- Plotly is an interactive and dynamic library for data visualization that supports a wide range of plot types and interactive features.

- PyWaffle enables you to visualize proportional representation using squares or rectangles.

- Matplotlib is one of the most widely used data visualization libraries in Python.

- Matplotlib was initially developed as an EEG/ECoG visualization tool.

- Matplotlib’s architecture is composed of three main layers: Backend layer, Artist layer, and the Scripting layer.

- The anatomy of a plot refers to the different components and elements that make up a visual representation of data.

- Matplotlib is a well-established data visualization library that can be integrated into different environments.

- Jupyter Notebook is an open-source web application that allows you to create and share documents.

- Matplotlib has a number of different backends available.

- You can easily include the label and title to your plot with plt.

- In order to start creating different types of plots of the data, you will need to import the data into a Pandas DataFrame.

- A line plot is a plot in the form of a series of data points connected by straight line segments.

- Line plot is one of the most basic types of charts and is common in many fields.

- You can generate a line plot by assigning "line" to 'Kind' parameter in the plot() function.
## Summary: Basic and Specialized Visualization Tools
- A pie chart is a circular statistical graphic, divided into segments, to illustrate numerical proportion.

- The process of creating a pie chart involves importing Matplotlib to represent a large set of data over a period of time.

- A box plot is a way of statistically representing given data distribution through five main dimensions.

- The five main dimensions are minimum, first quartile, median, third quartile, and maximum.

- You can create a box plot using Matplotlib.

- A scatter plot displays values pertaining to typically two variables against each other.

- The process of creating a scatter plot involves importing Matplotlib to visualize a large set of data.

- Matplotlib is a versatile plotting library that offers a flexible interface for creating various types of plots.

- Matplotlib’s Pyplot module offers a convenient way to create and customize plots quickly.

- Data Storytelling is the ‘art of storytelling’ that involves creating a narrative around the data.

- Data visualization is an important aspect of data storytelling and involves creating engaging visuals.
## Summary: Advanced Visualizations and Geospatial Data
- Folium is a data visualization library in Python that helps people visualize geospatial data.

- With Folium, you can create maps of different styles, such as street-level maps, stamen maps, and more.

- A feature of Folium is that you can create different map styles using the tiles parameter.

- With Folium, you can easily add markers on maps.

- The ‘location’ parameter specifies the latitude and longitude coordinates of the center point of the map.

- Markers play a vital role in enhancing interactivity and adding context to maps.

- The folium.Marker() function specifies location parameters.

- The popup parameter provides a label upon being clicked.

- Markers can be created using “feature group.”

- A choropleth map is a thematic map in which areas are shaded or patterned in proportion to the measurement of the statistical variable.

- When creating a choropleth map, Folium requires a GeoJson file that includes geospatial data of the region.

- The Mapbox Bright Tileset displays the name of every country when used on a map.
## Summary: Creating Dashboards with Plotly and Dash
- Dash is an Open-Source User Interface Python library for creating reactive, web-based applications.

- It is easy to build Graphical User Interfaces using Dash as it abstracts all technologies required to make the applications.

- There are two components of Dash: Core and HTML components.

- The dash_core_components describe higher-level interactive components generated with JavaScript, HTML, and CSS through the React.js library.

- The dash_html_components library has a component for every HTML tag.

- A callback function is a python function that is automatically called by Dash whenever an input component's property changes.

- The @app.callback decorator decorates the callback function in order to tell Dash to call it whenever there is a change in the input component value.

- The callback function takes input and output components as parameters and performs operations to return the desired result for the output component.
