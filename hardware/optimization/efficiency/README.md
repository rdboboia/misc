# TLDR
You can gain a lot of efficiency by:
- Lowering the default voltage.
- Limitting the default TDP.
- Fine tuning the frequency and voltage curves.

# What is efficiency
In simple terms the efficiency is the performance that we get for each power unit consumed. That is, efficiency is the performence per watt. The more performance per watt, the more efficient a component is.

In general, speaking of any component, there is always a sweet spot where the efficiency peaks.
However, in most cases, that peak is far from the ideal performance.
By tuning the performance and power draw we can gain efficiency by moving along the efficiency curve into a spot where the performance decrease is not noticeable but the power draw is a lot lower, which leads to improved efficiency at roughtly the same performance.

Without going in detail (since this is already tested and explained in each component's section) I found out that for NVIDIA 4000 and 5000 series GPUs we can reduce the power consumption by 25% while only loosing at most 5% performance, and for AMD 9000 series CPUs we can reduce the power consumption by 30% while maintaining the same performance (or reduce power consumption by 40% while only loosing 5% performance).

# Hardware efficiency optimizations
Modern hardware is pushed kinda hard from the factory, which leads to unnecessarily high voltages, temperatures and power consumption. The main motivation for this is to ensure that the expected performance is met by even the worst samples. However those samples that are not in that worst case have a lot of efficiency to be gained by tweaking some parameters, primarily the default frequency-voltage curve and the max allowed TDP.

You can find my analysis and conclusions for each hardware component in inner folders (WIP for now; will be available in some days).

# Disclaimer
We can tweak the hardware in any direction we want, not just for efficiency. However I will focus on that aspect as it is my main goal.

We must also take into account that the efficiency can vary depending on the specific load that we are using to benchmark the performance. My results are based on some specific application(s) that might or might not be the best overall representation, so I encourage you to test and tune your hardware to best suit your needs and most used applications.
