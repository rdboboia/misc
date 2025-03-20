# NVIDIA RTX 4070Ti Super

## Efficiency analysis
This should apply to NVIDIA's 4000 and 5000 series GPUs since they have a very similar architecture.

As you can see in the graph below the performance doesn't scale in the same amount as the TDP.
We only lose 1% performance for each 5% TDP reduction until 75%. Bellow 75% TDP the performance decrease is larger for each TDP step.
So, in my case, around 75% TDP is the ideal power reduction while maintaining roughtly the same performance (5% performance is not that noticeable).

For GPUs this is the easiest and fastest efficiency tunning method.
If we want to squish more efficiency (or restore some performance while using the TDP reduction) we can fine tune the voltage curve.
MSI Afterburner can do this automatically, which I recomment, with the OC scanner.
This can also be done with the NVIDIA's APP auto overclocking feature, but I don't like this method that much since it also overclocks the memory (we have less control in the NVIDIA's APP).

![image](https://github.com/user-attachments/assets/2f1d9857-0c1d-4ca4-adf4-f9332a2a9caf)
