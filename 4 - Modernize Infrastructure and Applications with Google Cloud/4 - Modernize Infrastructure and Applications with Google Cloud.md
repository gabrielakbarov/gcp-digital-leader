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