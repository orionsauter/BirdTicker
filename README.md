# BirdTicker
JavaScript tool to display the latest detections from a BirdWeather station.

On loading, the page Ticker will fetch the latest results from a given station using a GraphQL query. Currently, the code loads 1 page of data (set by `maxpage`), to save time. These results are displayed using [Tabulator](https://tabulator.info/), which formats them nicely, and could be used for sorting/filtering in the future. To change the target station, replace `station = "2707"` with the code for yours.

The page Stats creates histograms for each species using [Chart.js](https://www.chartjs.org/) showing the counts for the certainty values assigned by the PUC. The charts are sorted by the number of detections in descending certainty.

The BirdWeather app only shows detections of birds, and filters out those it deems unlikely. This viewer allows you to see the unfiltered detections, including non-bird sounds (such as engines and dogs) and spurious sounds associated with bonkers species (penguins in Michigan!).

## TODO:
- Better organization of charts on the page
- Better limiting of fetched data
- Add new charts for more visualizations
