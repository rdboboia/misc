# Hardware efficiency optimizations
Modern hardware is pushed kinda hard from the factory, which leads to unnecessarily high voltages, temperatures and power consumption. The main motivation for this is to ensure that the expected performance is met by even the worst samples. However those samples that are not in that worst case have a lot of efficiency to be gained by tweaking some parameters, primarily the default frequency-voltage curve and the max allowed TDP.

You can find my analysis and conclusions for each hardware component in inner folders (WIP for now; will be available in some days).

# Disclaimer
We can tweak the hardware in any direction we want, not just for efficiency. However I will focus on that aspect as it is my main goal.

We must also take into account that the efficiency can vary depending on the specific load that we are using to benchmark the performance. My results are based on some specific application(s) that might or might not be the best overall representation, so I encourage you to test and tune your hardware to best suit your needs and most used applications.

# TLDR
You can gain a lot of efficiency by:
- Lowering the default frequency-voltage curve.
- Limitting the default TDP.
- Tweaking the default frequency.
