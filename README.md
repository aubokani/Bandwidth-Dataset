# Mobile Network Bandwidth Dataset

### Overview
This dataset contains mobile network bandwidth traces collected from vehicular networks in Australia in 2015. The data was used in the following publication:

**Bokani, A., Hassan, M., Kanhere, S. S., Yao, J., & Zhong, G. (2016). Comprehensive mobile bandwidth traces from vehicular networks.** In *Proceedings of the 7th international conference on multimedia systems* (pp. 1–6). ACM.

The dataset consists of bandwidth measurements from both 3G and 4G networks, with detailed information such as download duration, download rate, location coordinates, and network operator details.

### Dataset Contents
The dataset includes two files:
1. **3G_BWData.json** - Contains bandwidth traces for 3G networks.
2. **4G_BWData.json** - Contains bandwidth traces for 4G networks.

Each file contains a list of results, where each entry represents a single bandwidth measurement session.

### File Structure
Each JSON file has the following structure:

```json
{
  "results": [
    {
      "countryISO": "au",             # Country code (ISO standard)
      "createdAt": "2015-03-25T01:30:26.966Z",  # Time of record creation (ISO 8601)
      "dateTime": "25/03/2015 12:30:22 PM",     # Local time of measurement
      "dlDuration": 1.21,             # Download duration in seconds
      "dlRate": 6770.247933884298,     # Download rate in kbps
      "dlSize": 8388608,               # Downloaded data size in bytes
      "endLat": -33.89607744,          # End latitude of the measurement
      "endLon": 151.19730279,          # End longitude of the measurement
      "lat": -33.89607744,             # Latitude of the measurement location
      "lon": 151.19730279,             # Longitude of the measurement location
      "networkType": 13,               # Network type (e.g., 13 = LTE)
      "objectId": "Tp1rIzPW4k",        # Unique object ID for the measurement
      "operatorCode": "50502",         # Mobile network operator code
      "operatorName": "amaysim",       # Mobile network operator name
      "subscriberID": "505025103462987", # Subscriber ID (anonymised)
      "updatedAt": "2015-03-25T01:30:26.966Z"  # Time of record update
    },
    ...
  ]
}
```

### Features
- **Location Information**: Each bandwidth trace contains latitude and longitude values for the point of measurement.
- **Network Types**: The `networkType` field indicates the type of network (e.g., 3G, 4G LTE).
- **Operator Details**: Includes the mobile network operator's name and code, which can be cross-referenced with public operator lists.
- **Download Metrics**: Each entry includes the download rate (`dlRate` in kbps), download size (`dlSize` in bytes), and download duration (`dlDuration` in seconds), providing detailed insights into network performance.

### Usage
Researchers can use this dataset to study:
- Network performance in vehicular environments.
- The variation in mobile bandwidth based on location, time, and network operator.
- Comparative analysis of 3G and 4G network performance in Australia.

### Citation
If you use this dataset, please cite the following paper:

Bokani, A., Hassan, M., Kanhere, S. S., Yao, J., & Zhong, G. (2016). Comprehensive mobile bandwidth traces from vehicular networks. In *Proceedings of the 7th international conference on multimedia systems* (pp. 1–6). ACM.

### Contact
For any queries or further information, please contact:

**Dr. Ayub Bokani**  
Email: aubokani@gmail.com
