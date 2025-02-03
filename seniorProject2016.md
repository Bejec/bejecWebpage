# Senior Project 2016: Real-time Data Analytics Pipeline

This project demonstrates

## Test youtube video embedding

<div class="video-container-16by9">
  <iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/GgMPIi-hsTo"></iframe>
</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/GgMPIi-hsTo" title="YouTube video player" frameborder="0" allowfullscreen></iframe>


## Project Goals

The main objectives of this project were:

* **Real-time Ingestion:** Capture streaming data from a high-volume source with minimal latency.
* **Real-time Processing:** Perform data transformations and aggregations in real-time.
* **Scalability and Reliability:** Ensure the pipeline can handle fluctuating data volumes and maintain high availability.
* **Actionable Insights:**  Provide real-time insights to inform business decisions.

## Architecture

The project utilizes several Google Cloud services to achieve these goals:

* **Data Source:** Simulated streaming data (could be replaced with a real-time source like Pub/Sub).
* **Data Ingestion:** Cloud Pub/Sub for reliable message delivery.
* **Stream Processing:** Cloud Dataflow for real-time data processing and transformations.
* **Data Storage:** BigQuery for storing processed data and enabling analytical queries.
* **Visualization:** Looker Studio (formerly Data Studio) for visualizing the results.

A simplified diagram of the architecture could be included here.  (Since I cannot access external resources, I can't create a visual diagram, but you would typically include one here in your `project-alpha.md` file).


## Key Technologies

* **Cloud Pub/Sub:**  Handles message ingestion and provides a scalable and reliable messaging service.
* **Cloud Dataflow:** Enables real-time data processing with built-in capabilities for windowing, aggregations, and transformations.
* **BigQuery:**  Provides a scalable data warehouse for storing and querying large datasets.
* **Looker Studio:**  Allows for creating interactive dashboards and visualizations to explore the processed data.

## Code Example (Conceptual)

While I cannot provide real code here, I can offer a conceptual example of a Dataflow pipeline:

