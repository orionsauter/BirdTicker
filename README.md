# BirdTicker
JavaScript tool to display the latest detections from a BirdWeather station.

On loading, the page will fetch the latest results from a given station using a GraphQL query. Currently, the code loads 10 pages, which takes a few seconds. These results are displayed using [Tabulator](https://tabulator.info/), which formats them nicely, and could be used for sorting/filtering in the future. To change the target station, replace `station = "2707"` with the code for yours.

The BirdWeather app only shows detections of birds, and filters out those it deems unlikely. This viewer allows you to see the unfiltered detections, including non-bird sounds (such as engines and dogs) and spurious sounds associated with bonkers species (penguins in Michigan!).
