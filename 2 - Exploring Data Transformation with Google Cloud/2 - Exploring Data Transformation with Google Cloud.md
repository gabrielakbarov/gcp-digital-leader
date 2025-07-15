# 2 - Exploring Data Transformation with Google Cloud

- [2.1 The Value of Data](#21-the-value-of-data)
- [2.2 Google Cloud Data Management Solutions](#22-google-cloud-data-management-solutions)
- [2.3 Making Data Useful and Accessible](#23-making-data-useful-and-accessible)

---

## 2.1 The Value of Data

<ul>
  <li><strong>Value & role of data</strong></li>
  <li>
    <strong>Basic data management concepts</strong>
    <ul>
        <li><strong>Database</strong> </li>
        <li><strong>Data warehouse</strong> </li>
        <li><strong>Data lake</strong> </li>
    </ul>
  </li>
  <li><strong>Create value through data</strong></li>
  <li><strong>Cloud to gain value from data</strong></li>
  <li> 
    <strong>Data value chain</strong>
    <p>Text</p>
    <details>
      <summary><strong>(Picture)</strong> Data Value Chain</summary>
      <img src="assets/Data%20Value%20Chain.png" alt="Data Value Chain"/>
    </details>
</li>
  <li><strong>Data governance</strong></li>
</ul>

## 2.2 Google Cloud Data Management Solutions
```mermaid
    graph TD 
      A{Data?}
      A --> |Unstructured| B[Cloud Storage]
      A --> |Structured or semi-structured| C{Workload?}
      C --> |Transactional|D{SQL or NoSQL?}
      C --> |Analytical|E{SQL or NoSQL?}
      D --> |SQL|F{Scalability?}
      D --> |NoSQL|G[Firestore]
      F --> |Local/regional|H[Cloud SQL]
      F --> |Global|I[Spanner]
      E --> |SQL|J[BiqQuery]
      E --> |NoSQL|K[Bigtable]
      
```

<ul>
    <li>Google Cloud data management solutions
        <table>
            <thead>
                <tr>
                    <th>Option</th>
                    <th>Data type</th>
                    <th>Characteristics</th>
                    <th>Use cases / examples</th>
                    <th>When to choose</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Cloud Spanner</td>
                    <td>Structured</td>
                    <td>Fully managed database service<br/>Unlimited scale (handles unexpected business spikes)<br/>Strong consistency<br/>High availability</td>
                    <td>Strong global consistency<br/>High I/O operations per second<br/>SQL relational database with joins</td>
                    <td></td>                
                </tr>
                <tr>
                    <td>Cloud SQL</td>
                    <td>Structured</td>
                    <td>Fully managed database service<br/>Migrate production database with minimal downtime via DMS</td>
                    <td></td>                    
                    <td>Don't need horizontal scaling<br/>Don't need a globally available system</td>
                </tr>
                <tr>
                    <td>BiqQuery</td>
                    <td>Structured</td>
                    <td>Fully managed data warehouse<br/>Built-in analysis tools, machine learning features<br/>SQL queries<br/>Works in a multi-cloud environment</td>
                    <td></td>
                </tr>
                <tr>
                    <td>Firestore</td>
                    <td>Semi-structured</td>
                    <td>No-SQL cloud database<br/>Flexible, horizontally scalable<br/>Stores Documents in Collections<br/>Offline data access</td>
                    <td>Nested objects, numbers, strings<br/>Automatic scaling</td>
                </tr>
                <tr>
                    <td>Cloud Bigtable</td>
                    <td>Semi-structured</td>
                    <td>No-SQL big data database service<br/>Handles massive workloads<br/>Low latency, high throughput</td>
                    <td>Google Search, Google Analytics, Google Maps, Gmail<br/>Internet of Things<br/>User analytics<br/>Financial analysis</td>
                    <td>More than 1TB of semi-structured data<br/>Fast data<br/>No-SQL data<br/>Real-time processing or machine learning on the data</td>                
                </tr>
                <tr>
                    <td>Cloud Storage</td>
                    <td>Unstructured</td>
                    <td>Fully managed, any amount and retrievals<br/>Data is managed as objects<br/>Interacts with web technologies (URLs as identifier)<br/>No predefined data model
                        <details>  
                            <summary>Storage classes</summary>
                                    <ol type="1">  
                                        <li>Standard Storage: Hot data (frequently accesses & briefly saved data)</li>
                                        <li>Nearline Storage: Once per month</li>
                                        <li>Coldline Storage: Once every 90 days</li>
                                        <li>Archive Storage: Once a year (best option for data accessed less than once a year</li>
                                    </ol>
                        </details>Autoclass
                    </td>
                    <td>Videos<br/>Pictures<br/>Audio recordings<br/>Website content<br/>Storing data for archival<br/>Distributing large data objects</td>
                    <td>Unlimited storage<br/>Worldwide access<br/>Low latency, high durability<br/>Geo-redundancy</td>
                </tr>
            </tbody>
        </table>
        <details>
            <summary>
                <strong>
                    (Picture)
                </strong> 
            Which Database should I use?
            </summary>
            <img src="assets/Which%20Database%20should%20I%20use.png" alt="Which Database should I use?"/>
        </details>
    </li>
    <li>Key data management concepts and terms</li>
    <li>Benefits of BiqQuery</li>
    <li>Modernizing a current database
        <ul>
            <li>Lift and shift</li>
            <li>Managed database migration</li>
        </ul>
    </li>
</ul>

## 2.3 Making Data Useful and Accessible

<ul>
    <li>Looker (democratizing access to data)</li>
    <li>BigQuery & Looker</li>
    <li>Real-time analytics</li>
    <li>Data pipelines within Google Cloud</li>
</ul>

