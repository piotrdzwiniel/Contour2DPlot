# Contour2DPlot
Simple plotting library written in Java and JavaFX, allowing for the creation of two-dimensional contour plot for two-dimensional data. Implementation is based on Marching Squares - https://en.wikipedia.org/wiki/Marching_squares#Isoband.

<h2>How to use?</h2>

All you need to do is to prepare `double[][] data` and create `Contour2DMap` object. Example use of this simple library can look like this:

```
Contour2DMap contour2DMap = new Contour2DMap(600, 600);    // Specify in the constructor width and height of the contour map.
contour2DMap.setData(data);    // Set data.
contour2DMap.setIsoFactor(1);    // Set iso factor, which is a step between subsequent iso values.
contour2DMap.setInterpolationFactor(10);    // Set interpolation factor.
contour2DMap.setMapColorScale("Color");    // Set contour map color scale - "Color" or "Monochromatic".
contour2DMap.draw();    // Draw all elements on the contour map.
```

`Contour2DMap` object inherits from `javafx.scene.layout.Pane`, so you can nest it in other `javafx.scene.layout.*` objects, such as `BorderPane`.

<h2>Screenshots</h2>

Contour2DPlot allows one to plot color and monochromatic maps.

![Image1](https://github.com/bluevoxel/Contour2DPlot/raw/master/screenshots/ContourPlotColor.png)

![Image2](https://github.com/bluevoxel/Contour2DPlot/raw/master/screenshots/ContourPlotMonochromatic.png)
