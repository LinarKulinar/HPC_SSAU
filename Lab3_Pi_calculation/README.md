# π computation by the Monte Carlo method on GPU and CPU
.ipynb был написан с помощью Google Colab
Для расспаралеливания использовалась библиотека PyCuda
Реализовано вычисление числа π методом Монте-Карло на CPU (на питоне с циклами for) и на GPU (на языке C с ипользованием билиотеки PyCuda)
В результате замеров времени выполнения работы на CPU/GPU было посчитано ускрение. Результаты изменений и значения числа π приведены в таблице ниже:
<table>
<thead>
<tr><th>Number of iterations</th><th>CPU time, s</th><th>GPU time, s</th><th>Acceleration</th><th>|our_cpu.π-numpy.π|</th><th>|our_gpu.π-numpy.π|</th></tr>
</thead>
<tbody>
<tr><td>2^25=33554432</td><td> 16.0495</td><td> 3.9079</td><td> 4.1069</td><td>0.00037601788575258865</td><td>0.00037601788575258865</td></tr>
</tbody>
</table>
