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
<tr><td>2^18=262144</td><td> 0.1219</td><td> 0.0062</td><td> 19.7453</td><td>0.002145139378956884</td><td>0.002145139378956884</td></tr>
<tr><td>2^22=4194304</td><td> 1.9411</td><td> 0.4428</td><td> 4.3835</td><td>0.0014480034536639153</td><td>0.0014480034536639153</td></tr>
<tr><td>2^25=33554432</td><td> 16.0495</td><td> 3.9079</td><td> 4.1069</td><td>0.00037601788575258865</td><td>0.00037601788575258865</td></tr>
</tbody>
</table>
