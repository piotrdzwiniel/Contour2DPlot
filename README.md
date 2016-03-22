# Contour2DPlot
<h4>Under GNU GPLv3 license (or later)</h4>
Simple plotting package written in Java and JavaFX, allowing for the creation of two-dimensional contour plot for two-dimensional data. Implementation is based on Marching Squares - https://en.wikipedia.org/wiki/Marching_squares#Isoband.

<h2>How to use?</h2>

All you need to do is to prepare `double[][] data` and create `Contour2DMap` object. Example use of this simple library can look like this:

```
// Specify in the constructor width and height of the contour map.
Contour2DMap contour2DMap = new Contour2DMap(600, 600);

// Specify size for the contour map container.
contour2DMap.setPrefSize(600, 600);

// Set data.
contour2DMap.setData(data);

// Set iso factor, which is a step between subsequent iso values.
contour2DMap.setIsoFactor(1);

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
