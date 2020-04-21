# Angles(interior and exterior) in regular polygons

## Using Gnuplot 

For a polygon with three sides, one can use gnuplot

Triangle 3 Sides
    
    set term dumb
    unset key
    set parametric
    set size square
    set xrange [-1:1]
    set yrange [-1:1]
    set samples 4
    plot [0:2*pi] sin(t),cos(t)
    set term svg
    set output "3.svg"
    replot
    reset

results in ![Triangle](/images/3.svg)

Now by changing the number following the command
    set samples N+1
where N is the polygon you want to draw.  For a square, the command becomes
    set samples 5
And the result will be
![Square](/images/4.svg)

The following pictures are in SVG format which means
Scalar Vector Graphics, a PNG represents Portable Network Graphics,
and so on.

![Pentagon](/images/5.svg)

![Hexagon](/images/6.svg)

![Heptagon](/images/7.svg)

![Octagon](/images/8.svg)

![Nonagon](/images/9.svg)

![Decagon](/images/10.svg)

## Using Metapost

    beginfig(1)
      n:=5;
      draw for i=0 step 1 until n-1:
        1cm*up rotated (i*360/n) --
      endfor cycle;
    endfig;
    end
Paste it in Troy Henderson's Metapost Previewer

![Pentagon-Metapost](/images/pentagon.svg)

You can change the 5 to a 6 and draw a hexagon. 
On your own you can cut and paste and use the metapost previewer

![http://www.tlhiv.org/mppreview/](http://www.tlhiv.org/mppreview/) 

Without using a protractor you can verify that the interior angles in a triangle measure 60 degrees, the exterior 120.  For a square both are 90 and for a pentagon, the angle measures 108 degrees and exterior is 72 degrees.

