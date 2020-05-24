# Thailand Covid-19 Infection Sources and Tracking Technology Analysis
Tracking and tracing is the main tool for detect and control Covid-19.  As of 24 May 2020, there are 3030 reported cases.  With social distancing and several measures implemented by Thai Government, we have passed the first wave and in the process of relaxing the control.  However, there are some concerns that the second wave may hit in the near future.

Several mobile apps have been developed in order to collect data and prepare for mitigating the risks of second wave.  The question remains what types of tracking technologies we should use: qr-code, gps, and bluetooth.  There are lots of discussions with arguments based on the feeling of effectiveness and privacy.  Using public cases data from DDC (https://covid19.ddc.moph.go.th/th/network), this analytics will determine the effectiveness of these technologies.

## Main Question
Given existing cases, how many cases can be detected by each technology?

## Main Assumptions
- qr code should be the prefered choice for known or specific *public* areas related cases
- bluetooth is suitable for close contact
- gps is suitable for *private* or *community/unknown* areas.

## Methodology
Based on the source of infection provided in the description and location in the DDC data, we classify infected cases into the following categories:
- 'closed_contacts': infected from being near infected patients
- 'medical_services': infected due to working in the medical facilities
- 'abroad': travelling from abroad
- 'unknown': infected without causes
- 'local': infected from the community without specific location (e.g. in provinces, etc.)
- 'crowded': infected from crowded and known places
- 'airports': infected from working at the airport
- 'public_transports': infected from public transports (e.g. taxi drivers)
- 'traveller': infected from oversea traveller
- 'in_progress': still under investigation

## Results
**Out of 2672 cases**

Category|Number of cases|Preferred Technology
---|---|---
closed_contacts|791|Bluetooth
in_progress|570|N/A
crowded|562|QR Code
abroad|446|No need (Quarantine)
unknown|157|N/A
medical_services|82|QR Code
local|26|GPS
friend_family|15|GPS
traveller|14|GPS
airports|5|QR Code
public_transports|4|GPS

## Conclusion
For 3 tracking technolgies, Bluetooth is the best with 52% coverage.  QR code will be able to help detecting only 43% of all cases.  GPS can complete the picture for residence or private areas.  Thus, if there is the second wave, data from qr code checkin alone will not be enough.
