# DevOps-Guide-2024
<h1>My DevOps Journey and Contributions</h1>

<h2>Introduction</h2>
<p>When I began exploring DevOps, I was completely new to the field and unfamiliar with core concepts and tools like GitHub Actions, Kubernetes, and infrastructure as code. However, learning DevOps through this course has been transformative. It has equipped me with essential skills, deepened my understanding of modern software practices, and enabled me to work on hands-on projects that bridge development and operations seamlessly.</p>

<h2>My Journey So Far</h2>

<h3>Early Stages: Understanding DevOps</h3>
<p>At the start, my knowledge of DevOps was limited. I didn’t fully grasp the importance of automation, collaboration, and continuous integration/continuous deployment (CI/CD) pipelines. But as I progressed through the course, I quickly saw how DevOps principles and tooling could streamline workflows, improve productivity, and ensure reliable deployments.</p>
<p>One of the biggest milestones was becoming comfortable with GitHub Actions. Initially, it felt overwhelming, but I soon learned to automate tasks and manage deployments directly from GitHub, which became a powerful tool in my development workflow.</p>

<h3>Key Projects and Hands-On Experience</h3>

<ul>
    <li>
        <strong>Deployment of Final Year Project using GitHub Actions</strong>
        <p>One of my proudest accomplishments was deploying my final year project, <em>Hallucination Detection on Large Language Models (LLMs)</em>, using GitHub Actions. This project involved complex machine learning workflows, and deploying it successfully required a robust CI/CD pipeline.</p>
        <p>GitHub Actions allowed me to automate testing, integrate seamlessly with Docker for containerization, and deploy updates smoothly, improving efficiency and reliability.</p>
    </li>
    <li>
        <strong>Current Project: Web Application Deployment with GitHub Tooling</strong>
        <p>I am currently deploying another web application using GitHub tooling, which is further enhancing my understanding of deployment pipelines and automation. Working on this project has allowed me to refine my skills and gain hands-on experience with different stages of the DevOps lifecycle.</p>
    </li>
</ul>

<h2>Skills and Knowledge Gained</h2>

<h3>1. Kubernetes</h3>
<p>I now have a solid understanding of <strong>Kubernetes</strong>, including how to manage and deploy applications in containerized environments. Kubernetes’ orchestration capabilities allow for managing complex applications with ease, from scaling to maintaining high availability.</p>

<h3>2. Knative</h3>
<p>Through working with Knative, I’ve learned how to handle serverless deployments on Kubernetes. This tool simplifies the deployment of containerized apps and offers powerful event-driven scaling, which is particularly useful for applications with fluctuating demand.</p>

<h3>3. Terraform</h3>
<p><strong>Terraform</strong> introduced me to the concept of Infrastructure as Code (IaC). Using Terraform, I can define infrastructure configurations in a declarative manner, making it easy to manage, share, and version control the entire infrastructure setup.</p>

<h3>4. Docker and Containerization</h3>
<p>Docker has become fundamental to my DevOps journey. I’ve learned to containerize applications, making them portable, consistent, and easier to deploy across various environments. Combining Docker with Kubernetes has enabled me to deploy complex, scalable applications with ease.</p>

<h3>5. GitHub Actions</h3>
<p>GitHub Actions has been central to automating workflows. From automating tests to deploying updates, GitHub Actions has streamlined repetitive tasks, ensuring consistency and enabling me to focus on core development.</p>

<h2>Challenges and Solutions</h2>
<p>DevOps is a challenging field, and I’ve faced my share of obstacles. Setting up Kubernetes for the first time, troubleshooting containerization issues, and configuring CI/CD pipelines presented significant learning curves. However, these challenges provided valuable learning experiences, teaching me critical troubleshooting skills and deepening my understanding of system configurations and optimizations.</p>

<h2>Future Goals</h2>
<p>Looking forward, I’m excited to further enhance my DevOps expertise. My next steps include:</p>
<ul>
    <li>Pursuing certifications such as the <em>Kubernetes and Cloud Native Associate (KCNA)</em> to validate my skills.</li>
    <li>Delving deeper into advanced topics like monitoring and observability, service mesh integrations, and cloud-native security.</li>
    <li>Contributing to open-source projects and actively engaging with the DevOps community to continue my learning and share my insights.</li>
</ul>

<h2>Additional Resources</h2>
<p>For anyone interested in learning more about DevOps, I recommend the following resources:</p>
<ul>
    <li><a href="https://kubernetes.io/docs/">Kubernetes Documentation</a></li>
    <li><a href="https://developer.hashicorp.com/terraform/docs">Terraform Documentation</a></li>
    <li><a href="https://docs.github.com/en/actions">GitHub Actions Documentation</a></li>
    <li><a href="https://docs.docker.com/">Docker Documentation</a></li>
</ul>

<h1>==========================================================================================</h1>


# Blog Summaries

## Blog 1: **Using Terraform to Deploy AWS EKS**

In this blog, we explored how to use **Terraform**, a popular Infrastructure as Code (IaC) tool, to deploy an **Amazon Elastic Kubernetes Service (EKS)** cluster. The blog highlighted the following steps and benefits of using Terraform for EKS deployments:

1. **Infrastructure as Code (IaC)**: By defining infrastructure as code with Terraform, teams can automate and manage their Kubernetes infrastructure with consistency across environments. This IaC approach minimizes manual errors and improves operational efficiency, allowing for a more organized and trackable setup.

2. **Scalability and Automation**: Terraform simplifies scaling by allowing users to modify infrastructure configurations quickly. With Terraform’s declarative syntax, making changes to infrastructure—like adding nodes to the EKS cluster—is straightforward and can be applied across environments, ensuring a smooth and automated scaling process.

3. **Consistent, Version-Controlled Infrastructure**: Terraform allows for version control of infrastructure, which means that any change to the infrastructure can be tracked, rolled back if necessary, and replicated consistently across environments. This provides a robust and repeatable approach to managing Kubernetes clusters in production environments.

4. **Hands-on Walkthrough**: The blog provided a practical walkthrough, guiding readers through the setup process of an EKS cluster using Terraform, covering configuration, cluster initialization, and deploying basic workloads.

### Key Takeaway
Using Terraform to deploy AWS EKS streamlines Kubernetes cluster management, making it scalable, consistent, and easy to modify as applications grow. By following this setup, users can deploy and manage Kubernetes workloads seamlessly, bringing the benefits of automation and IaC to their cloud infrastructure.

---

## Blog 2: **Autoscaling Containers in Kubernetes**

This blog delved into the crucial role of **autoscaling** in Kubernetes and how it contributes to high availability and cost-efficiency for modern, containerized applications. Autoscaling ensures that resources are allocated based on real-time demand, improving application performance and resource optimization. The key points covered include:

1. **Types of Autoscaling in Kubernetes**:
   - **Horizontal Pod Autoscaler (HPA)**: The HPA automatically adjusts the number of pod replicas in a deployment based on CPU utilization or custom metrics, making it ideal for handling spikes in demand. This flexibility ensures that applications have the right amount of resources when traffic surges.
   - **Vertical Pod Autoscaler (VPA)**: VPA adjusts the CPU and memory limits of individual pods, rather than adding new replicas, to ensure each pod has the optimal amount of resources based on historical usage and demand.
   - **Cluster Autoscaler**: The Cluster Autoscaler adds or removes nodes in a cluster based on pending pod requests, helping to prevent resource shortages and improving the cluster's responsiveness to changing workloads.

2. **Monitoring and Load Balancing**:
   - To effectively implement autoscaling, monitoring tools are essential to collect metrics on application usage and performance. Integrated monitoring tools, along with Kubernetes metrics, provide visibility into application health and help fine-tune autoscaling parameters.
   - Load balancers distribute incoming requests across pods and nodes, ensuring even distribution and efficient resource use. By pairing autoscaling with load balancing, applications remain resilient and responsive under varying traffic levels.

3. **Benefits of Autoscaling**:
   - **High Availability**: Autoscaling helps maintain high availability by ensuring that applications have the necessary resources during traffic surges. This minimizes downtime and improves user experience.
   - **Cost-Efficiency**: Autoscaling optimizes resource usage by scaling down during low-demand periods, preventing waste of resources and reducing operational costs.
   - **Scalability and Resilience**: Autoscaling enables applications to dynamically respond to demand changes, providing a more robust and flexible infrastructure that can adapt to traffic patterns in real time.

### Key Takeaway
Autoscaling in Kubernetes, through tools like HPA, VPA, and Cluster Autoscaler, allows organizations to create resilient and scalable applications that respond dynamically to real-time changes in traffic. This ensures high availability and optimizes resource usage, balancing cost efficiency with performance for a well-managed, modern infrastructure.

<h1>==========================================================================================</h1>

<h1>Sample repo from the internet and applying DevOps tooling</h1>
# Automating Web Application Deployment with GitHub Actions and GitHub Pages

Understanding what it takes to deploy web applications both securely and efficiently is vital for any organization. In this educational module, **TELUS** and **Amplifon** will provide expert insights as we move through the steps for automating application deployment using **GitHub Actions** and **GitHub Pages**. Follow along with a copy of our demo repository to learn and practice each step.

By the end of this pathway, we will have learned the basics of **GitHub Actions** and understand how to use workflows to build, test, and deploy an application.

**Project Repository:** [GitHub Actions Learning Pathway](https://github.com/aftab0575/actions-learning-pathway)

## Overview

For this module, we'll work with a sample **Next.js** application, which serves as a practical example for understanding the deployment process end-to-end.

### Prerequisites
- A GitHub account
- Basic knowledge of GitHub (e.g., how to navigate to the Actions tab, open, and edit files)
- Familiarity with YAML files or a willingness to learn (as GitHub Actions configurations are written in YAML)

---

## Essentials Module Overview

### Guide 1: Building a Workflow with GitHub Actions
Kickstart your automation journey by copying a demo repository and building your first GitHub Actions **"Hello World!"** workflow. This guide provides a step-by-step process to get you started with GitHub Actions.

### Guide 2: Building an Application with GitHub Actions
Learn the basics of using GitHub Actions to build an application—a common step in any **CI/CD pipeline**. Explore reusing prebuilt actions from **GitHub Marketplace** to save time and effort in the development process.

### Guide 3: Testing Applications with GitHub Actions
Automate testing with GitHub Actions and utilize prebuilt actions from GitHub Marketplace to run a variety of third-party testing tools. This guide will also help you understand the difference between **GitHub-hosted** and **self-hosted runners**, and when to use each option.

### Guide 4: Configure Your Deployment Environments in GitHub
Learn to set up deployment environments to create deployment targets for various purposes, such as staging and production. You'll also enable GitHub Pages before deployment.

### Guide 5: Automating and Deploying Workflows with GitHub Actions
Deploy a **Next.js static site** to **GitHub Pages** using GitHub Actions. This guide will walk you through building, testing, and deploying the application as a fully automated process.

---
## Skills and Tools Used

- **GitHub Actions**: Create automated workflows for building, testing, and deploying applications.
- **GitHub Pages**: Host and deploy static websites directly from a GitHub repository.
- **YAML**: Configuration language for GitHub Actions workflows.
- **Next.js**: Framework used for building the demo application and understanding deployment.
- **CI/CD Concepts**: Continuous Integration and Continuous Deployment principles applied to workflow automation.
- **Testing Tools**: Using third-party testing actions from GitHub Marketplace.
- **Environment Management**: Setting up deployment environments (e.g., staging and production) for different deployment stages.

