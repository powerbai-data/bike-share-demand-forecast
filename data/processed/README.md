
## Processed Data Description

The processed dataset is constructed by combining 18 months of raw Divvy trip-level CSV files into a single table.

During processing, only the columns required for the time series analysis were retained.  
The original raw data contains one row per individual trip.

To support time series modeling, the data was aggregated from trip-level to daily-level:
- Trips were grouped by date
- Daily ride counts were computed
- The resulting dataset contains one row per date

The final processed dataset is indexed and sorted by date, making it suitable for time series analysis and forecasting.

This transformation significantly reduces data volume while preserving the temporal demand structure required for seasonal analysis and forecasting.
