# Contour2DPlot
<h4>Under GNU GPLv3 license (or later)</h4>
Simple plotting package written in Java and JavaFX, allowing for the creation of two-dimensional contour plot for two-dimensional data. Implementation is based on Marching Squares - https://en.wikipedia.org/wiki/Marching_squares#Isoband.

<h2>How to use?</h2>

In order to use package in your project you have to copy and paste `org.contour2dplot.*` to the project's location. Now, after including imports in your class, all you need to do is to prepare `double[][] data` and create `Contour2DMap` object. Example use can look like this:

```
// Specify in the constructor width and height of the contour map.
Contour2DMap contour2DMap = new Contour2DMap(600, 600);

// Specify size for the contour map container.
contour2DMap.setPrefSize(600, 600);

// Set data.
contour2DMap.setData(data);

// Set iso factor, which is a step between subsequent iso values.
contour2DMap.setIsoFactor(1.0);

// Set interpolation factor.
contour2DMap.setInterpolationFactor(10);

// Set contour map color scale - "Color" or "Monochromatic".
contour2DMap.setMapColorScale("Color");

// Draw all elements on the contour map.
contour2DMap.draw();    
```

`Contour2DMap` object inherits from `javafx.scene.layout.Pane`, so you can nest it in other `javafx.scene.layout.*` objects, such as `BorderPane`.

<h2>Screenshots</h2>

Contour2DPlot allows one to plot color and monochromatic maps.

![Image1](https://github.com/bluevoxel/Contour2DPlot/raw/master/screenshots/Contour2DMapColor.png)

![Image2](https://github.com/bluevoxel/Contour2DPlot/raw/master/screenshots/Contour2DMapMonochromatic.png)

<hr>

<h1>How can I cite Contour2DPlot?</h1>

Contour2DPlot was created because I was lacking of an appropriate visualization tool for my Specvis project (https://github.com/piotrdzwiniel/Specvis). So if you find Contour2DPlot useful for your work/study/research please consider to cite the paper given below:

<ul>
    <li style="color: #FF2E2E;">In the near future this text will morph into a reference to the publication.</li>
</ul>

Why I ask you to cite Contour2DPlot by citing Specvis? Well, to be honest, citing it gives me some credit for its creation and motivate me to continue its development. But citing it is also important for a different reason - if you had found Contour2DPlot and/or Specvis useful, it would be desirable to share knowledge about it with others, so it can get to as many people as possible and serve well wherever it's needed.

Piotr Dzwiniel.
