<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>

<h1>ETL Workflow Project - Apple_Analysis</h1>

<p>This project implements an ETL (Extract, Transform, Load) pipeline designed to analyze customer data, specifically focusing on purchases related to iPhone and AirPods. The project is organized into three main stages: Extraction, Transformation, and Loading.</p>

<h2>Project Structure</h2>

<ul>
    <li><strong>Extract:</strong> The extraction process is handled by the <code>reader_factory</code> and <code>extractor</code> components.
        <ul>
            <li><code>reader_factory</code>: Responsible for identifying and reading the file type.</li>
            <li><code>extractor</code>: Extracts the data using the <code>reader_factory</code>.</li>
        </ul>
    </li>
    <li><strong>Transform:</strong> The transformation of the extracted data is managed by the <code>transform</code> component, which cleans, processes, and prepares the data for loading.</li>
    <li><strong>Load:</strong> The loading process is executed by the <code>loader_factory</code> and <code>loader</code> components.
        <ul>
            <li><code>loader_factory</code>: Determines the file type for loading.</li>
            <li><code>loader</code>: Loads the transformed data into a Delta Lake table on DBFS.</li>
        </ul>
    </li>
</ul>

<h2>Main Function</h2>

<p>The main function, <code>Apple_Analysis</code>, orchestrates the entire ETL pipeline. It has two primary workflows:</p>

<ol>
    <li><strong>AirPodsAfterIphone:</strong> Identifies customers who purchased AirPods after buying an iPhone.</li>
    <li><strong>OnlyAirpodsAndIphone:</strong> Identifies customers who purchased only AirPods and iPhone.</li>
</ol>

<h2>Getting Started</h2>

<p>To run the project, follow these steps:</p>

<ol>
    <li>Clone the repository:</li>
    <pre><code>git clone https://github.com/yourusername/your-repo-name.git</code></pre>
    <li>Navigate to the project directory:</li>
    <pre><code>cd your-repo-name</code></pre>
    <li>Run the main function:</li>
    <pre><code>python main.py</code></pre>
</ol>

<h2>Requirements</h2>

<p>Ensure you have the following dependencies installed:</p>

<ul>
    <li>Python 3.x</li>
    <li>pandas</li>
    <li>pyspark</li>
    <li>delta</li>
    <li>Any other dependencies relevant to your project</li>
</ul>

<h2>Contributing</h2>

<p>If you'd like to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue to discuss what you would like to change.</p>

<h2>License</h2>

<p>This project is licensed under the MIT License. See the <code>LICENSE</code> file for details.</p>

</body>
</html>









