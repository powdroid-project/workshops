# Introduction
In this workshop, we will try to benchmark Android apps in black box mode. As a reminder, the net energy consumed by an app can be defined as follows:

$E_{net} = E_{raw} - (P_{idle} \ast T_{measure})$

# Benchmark your Smartphone when idle

Before starting, we will estimate the power consumption in idle mode, referred to as $P_{idle}$. Run a PowDroid benchmark without using your smartphone, but after first preventing the screen from going into sleep mode. Calculate $P_{idle}$, which is the average of the values in the `Power` column of the CSV file. The more values there are, the better.

# Benchmark few popular apps

Choose two apps from the same functional family (e.g., web browsers). Run a PowDroid benchmark for each app, using a specific and well-defined scenario. Then calculate $E_{raw}$, which is the sum of the `Energy` column in the CSV file. Also calculate $T_{measure}$, which is the total duration of your benchmark, using the `start_time` and `end_time` columns. 

Repeat this benchmark at least 5 times for each app, under identical conditions.

# Awesome data vizualisation

For each app, you therefore have at least 5 net energy values $E_{net}$, bearing in mind that $E_{net} = E_{raw} - (P_{idle} \ast T_{measure})$. Basically, we subtract the energy consumed by the device itself to isolate the energy consumed by the app alone.

Visually represent the data points for “App1” and “App2” using a statistical graph such as a BoxPlot or ViolinPlot. You can use Excel or any other more suitable software.

So, which app consumes the least energy? 🏆


# Share your results with the world

Make a Pull Request to add your data to the dedicated [crowdsourcing](../crowdsourcing/) repository
