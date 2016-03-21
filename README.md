# Contour2DPlot
Custom, simple plotting library, allowing for displaying 2D contour plot for two-dimensional data. Implementation is based on https://en.wikipedia.org/wiki/Marching_squares#Isoband.

<h2>How to use?</h2>

All you need to do is to prepare `double[][] data` and create `Contour2DMap` object. Example use of this simple library can look like this:

```
Contour2DMap contour2DMap = new Contour2DMap(600, 600);
contour2DMap.setData(data);
contour2DMap.setIsoFactor(1);
contour2DMap.setInterpolationFactor(10);
contour2DMap.setMapColorScale("Color"); // or "Monochromatic".
contour2DMap.draw();
```

`Contour2DMap` object inherits from `javafx.scene.layout.Pane`, so you can nest it in other `javafx.scene.layout.*` objects, such as `BorderPane`.

<h2>Screenshots</h2>

Contour2DPlot allows one to plot color and monochromatic maps.

![Image1](https://github.com/bluevoxel/Contour2DPlot/raw/master/screenshots/ContourPlotColor.png)

![Image2](https://github.com/bluevoxel/Contour2DPlot/raw/master/screenshots/ContourPlotMonochromatic.png)
