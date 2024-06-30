<h1>🚀 DevOps - Kubernetes Deployment of Clickhouse & Superset</h1>

![](https://as1.ftcdn.net/v2/jpg/05/12/04/52/1000_F_512045284_gsbCu75oyqHo59MccBltJe0sJRck1PPa.jpg)

<h2>📄 Overview</h2>
<p>This repository contains the Kubernetes configuration files for deploying Clickhouse and Apache Superset on Minikube. The objective of this assignment is to set up a stateful Clickhouse deployment with persistent storage and deploy Superset, a business intelligence tool, to create reports and charts based on data from Clickhouse.</p>

<h2>📋 Prerequisites</h2>
<ul>
    <li>🌐 Basic knowledge of Kubernetes and Docker</li>
    <li>🖥️ Minikube installed on your local machine</li>
    <li>📚 Familiarity with Clickhouse and Superset</li>
</ul>

<h2>⚙️ Steps to Deploy</h2>
<ol>
    <li><strong>🚀 Deploy Clickhouse</strong>
        <p>Create a StatefulSet for Clickhouse with a persistent storage of 10GB. Expose the native port 9000 for Superset to connect.</p>
    </li>
    <li><strong>📊 Deploy Superset</strong>
        <p>Create a Deployment for Superset. The configuration includes environment variables for the initial setup.</p>
    </li>
    <li><strong>🌐 Access Superset</strong>
        <p>Open Superset in your browser:</p>
        <pre><code>minikube service superset</code></pre>
    </li>
    <li><strong>🔗 Connect Clickhouse to Superset</strong>
        <p>
            <ol>
                <li>Go to the Superset URL in your browser.</li>
                <li>Navigate to <strong>Data &gt; Databases &gt; (+ Database button)</strong>.</li>
                <li>Choose Clickhouse from the list.</li>
                <li>Add the Clickhouse URL: <code>clickhouse://default@&lt;Clickhouse-Service-Name&gt;:9000/default</code></li>
                <li>Click <strong>Connect</strong>.</li>
            </ol>
        </p>
    </li>
</ol>

<h2>📝 Submission Details</h2>
<p>All YAML files are placed in the root directory for ease of testing. The configurations are uploaded to this GitHub repository.</p>

</body>
</html>
