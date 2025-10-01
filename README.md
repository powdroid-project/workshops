# Introduction
In this workshop, we will try to benchmark Android apps in black box mode. As a reminder, the net energy consumed by an app can be defined as follows:

$E_{net} = E_{raw} - (P_{idle} \ast T_{measure})$

# Smartphone benchmark when idle

Before starting, we will estimate the power consumption in idle mode, referred to as $P_{idle}$. Run a PowDroid benchmark without using your smartphone, but after first preventing the screen from going into sleep mode. Calculate $P_{idle}$, which is the average of the values in the `Power` column of the CSV file. The more values there are, the better.

# Benchmarking popular apps

Choose two apps from the same functional family (e.g., web browsers). Run a PowDroid benchmark for each app, using a specific and well-defined scenario. Then calculate $E_{raw}$, which is the sum of the `Energy` column in the CSV file. Also calculate $T_{measure}$, which is the total duration of your benchmark, using the `start_time` and `end_time` columns. 

Repeat this benchmark at least 5 times for each app, under identical conditions.

# Share your results with the world

Make a Pull Request to add your data to the dedicated [crowdsourcing](../crowdsourcing/) repository
