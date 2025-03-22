# 9800x3D

## Efficiency analysis
This should apply to all Ryzen 9000 series CPUs and could also have some impact in the previous (7000 series) CPU generation.

Tuning for CPU efficiency can be a little more tricky that for a GPU since there is no automated tool to auto optimize the frequency and voltage at the same time, but we can tune them both manually. However we must take into account that setting to low of a voltage can lead to instabilities, but there is no risk of damaging the hardware while undervolting.

The first step that I recommend doing is tuning the voltage curve for the default frequencies.
This can be easily done on AM5 by using a negative curve optimizer (CO) value.
In my case the CO can be up to -35. This sets the voltage back arount 0.2v, which is a huge decrease.
With this decrease in voltage comes a significant power draw and temperature decrease.
By just doing this we gain around 33% efficiency (same performance but 28% less power consumption, going from 125W stock to 90W).
For most users and cases I would stop tuning here.

However, if we want to fine tune the frequency and max allowed power consumption we can apply a power limit.
In my case I set it to around 80W, which seems like a good compromise to keep 96% of the performance at 64% of the original power draw (note that this will vary depending on the load).
I also limited the max 1 core and all core frequency to 5GHz.
I personally like have both 1 and all core frequencies to be the same.
This also ensures that, since no extra frecuency is used, the 1 core and all core load voltages will be the same, which in my case howers around 1v, which is a lot lower than the default voltage of ~1.22v.


![image](https://github.com/user-attachments/assets/15c0c42d-c15b-4462-800a-1a2f4718b1d2)
![image](https://github.com/user-attachments/assets/f2f984cb-c2ff-4e06-8467-a738b0a903cd)
