# esp32s3-ULP-ADC-Joe
 Reading Current sensor values using ESP32-S3 ADC

This code demonstrates how to use the ULP-RISC-V coprocessor to poll the ADC in deep sleep.

The ULP program periodically measures the input voltage on ADC1 channel 0, GPIO1 on ESP32-S3. The voltage is compared to an upper threshold. If the voltage is higher than the threshold, the ULP wakes up the system.


## Example output

Below is the output from this example.

```
Not a ULP-RISC-V wakeup (cause = 0), initializing it!
Entering in deep sleep

ULP-RISC-V woke up the main CPU
Threshold: high = 2000
Value = 4095 was above threshold
Entering in deep sleep
```

