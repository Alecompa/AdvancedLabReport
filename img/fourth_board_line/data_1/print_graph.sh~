#!/usr/bin/gnuplot -persist
file = 'calib_11'
type_out = '.png'
output = file.type_out
f(x) = a + b*x
fit f(x) file using 1:2:3 via a, b
set xrange [0:1.6]
set xlabel 'Voltage (V)'
set ylabel 'Channel'
set grid
set key left
set terminal pngcairo
set output output
set xzeroaxis
plot file using 1:( $2 - f($1) ):3 with yerrorbars title 'Data'
exit
