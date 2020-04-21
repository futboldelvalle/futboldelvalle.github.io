# Angles(interior and exterior) in regular polygons

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

