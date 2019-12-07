#!/usr/bin/gnuplot -persist
n = '3'
file = '_res_am'
type_out = '.png'
cable = 'Cable '
title_plot = cable.n
file_name = n.file
output = n.file.type_out
set xlabel 'Channel Number'
set ylabel 'Resolution (%)'
set grid
set offsets 1, 1, 0.1, 0.1
set terminal pngcairo
set output output
plot file_name using 1:2:3 with yerrorbars title title_plot 
exit
