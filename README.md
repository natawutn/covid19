# Thailand Covid-19 Infection Sources and Tracking Technology Analysis
Tracking and tracing is the main tool for detect and control Covid-19.  As of 24 May 2020, there are 3030 reported cases.  With social distancing and several measures implemented by Thai Government, we have passed the first wave and in the process of relaxing the control.  However, there are some concerns that the second wave may hit in the near future.

Several mobile apps have been developed in order to collect data and prepare for mitigating the risks of second wave.  The question remains what types of tracking technologies we should use: qr-code, gps, and bluetooth.  There are lots of discussions with arguments based on the feeling of effectiveness and privacy.  Using public cases data from DDC (https://covid19.ddc.moph.go.th/th/network), this analytics will determine the effectiveness of these technologies.

## Main Question
Given existing cases, how many cases can be detected by each technology?

## Main Assumptions
- qr code should be the prefered choice for known or specific *public* areas related cases
- bluetooth is suitable for close contact
- gps is suitable for *private* or *community/unknown* areas.

## Conclusion
For 3 tracking technolgies, QR code will be able to help detecting only 43% of all cases. Thus, if there is the second wave, data from qr code checkin alone will not be enough.
