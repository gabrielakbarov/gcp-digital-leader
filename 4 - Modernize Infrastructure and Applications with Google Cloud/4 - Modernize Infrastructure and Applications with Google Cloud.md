# 4 - Modernize Infrastructure and Applications with Google Cloud

- **Workload**: Specific application, service or capability that can be run in the Cloud or on premises.
<table>
    <th>Cloud Migration Term</th>
    <th>What it means</th>
    <th>Reason</th>
    <th>Example</th>
    <tr>
        <td>Retired</td>
        <td>No longer needed<br/>Shut down permanently</td>
        <td>Outdated<br/>Redundant<br/>Replaced</td>
        <td>An old internal tool without current usage</td>
    </tr>
    <tr>
        <td>Retained</td>
        <td>Workload is kept on-premises (temporarily or permanently)</td>
        <td>Compliance regulations<br/>Low migration priority<br/>Technical constraints</td>
        <td>Legacy system tightly coupled with on-prem hardware</td>
    </tr>
    <tr>
        <td>Rehosted<br/>("Lift and Shift")</td>
        <td>Moving the workload from on-premises to the cloud without making changes on the code or architecture</td>
        <td>Fast<br/>Simple<br/>Often used for early-stage migration</td>
        <td>Migrating a VM from on-premises to Compute Engine VM without changing the VM</td>
    </tr>
    <tr>
        <td>Replatform</td>
        <td>Migrating to the cloud and making some changes in code or architecture in order to better fit in the cloud</td>
        <td>Take advantage of cloud benefits without full redesign</td>
        <td>Moving from a self-managed database to Cloud SQL</td>
    </tr>
    <tr>
        <td>Refactored</td>
        <td>The workload is redesigned to fully exploit cloud-native features</td>
        <td>Scalability<br/>Performance<br/>Modernization</td>
        <td>Breaking a workload into microservices</td>
    </tr>
    <tr>
        <td>Reimagined</td>
        <td>The workload is completely rebuilt, often using cloud-native capabilities or SaaS</td>
        <td>Meet new business needs<br/>Completely modernize</td>
        <td>Replacing a custom system with a new solution using Firebase and AI APIs</td>
    </tr>
</table>

## Modernizing Infrastructure in the Cloud
- Total Cost of Ownership (TCO)
- **Benefits of running compute workloads in the cloud:** 
  - Pay-as-you-go model
  - Long-term commitment discounts
  - Scalability
  - Reliability, high uptime
  - Security (physical & cloud)
  - Flexibility
  - Abstraction 


- Virtual Machines:
  - Compute Engine

<ul>
    <li>Containers:
        <table>
            <tr>
                <td>Google Cloud Engine</td>
                <td>Cloud Run</td>
            </tr>
            <tr>
                <td>Provides lots of control over a Kubernetes environment<br/>with complex applications to run</td>
                <td>A simple, fully managed serverless platform<br/>that can scale up and down quickly.</td>
            </tr>
        </table>
    </li>
</ul>

<ul>
    <li>Serverless computing
        <table>
            <th>Product</th>
            <th>Explanation</th>
            <th>Example</th>
            <tr>
                <td>Cloud Run</td> 
                <td>Fully managed environment<br/>Run containerized applications</td>
            </tr>
            <tr>
                <td>Cloud Run functions</td> 
                <td>Platform for hosting simple, single-purpose functions<br/>Attached to events from cloud infrastructure or services</td>
                <td>Sending a notification when a new order is placed</td>
            </tr>
            <tr>
                <td>App engine</td> 
                <td>Service to build and deploy web applications</td>
                <td></td>
            </tr>
        </table>
    </li>
</ul>

- **Benefits of serverless computing:** 
  - Reduced operational costs
  - Scalability
  - Faster time-to-market
  - Reduced development costs
  - Improved resilience
  - Pay-per-use pricing model

## Modernizing Applications in the Cloud
- Application: Computer program or software that helps user do anything
- Benefits of modern cloud application development:
  - Flexible
  - Scalable
  - Uses latest technologies
  - High availability (load balancing, automatic failover
  - Monitoring and management tools)

- Apigee API Management (manage APIs: authentication, authorization, tracking and analyzing, developing, deploying, versioning, documentation)

- Hybrid Cloud
- Multi-Cloud
- GKE Enterprise
  - Multi-CLoud and Hybrid-CLoud support
  - Centralized management
  - Security and compliance
  - Networking and load balancing
  - Monitoring and logging
  - 