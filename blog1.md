# Introduction

GitOps has become increasingly popular as a way to manage cloud infrastructure and application deployments. The GitOps approach involves using Git as a single source of truth for infrastructure and application code, and using a pull-based approach to deployment to ensure that the desired state of the infrastructure is always reflected in Git.

While GitOps has proven to be a powerful approach for managing Kubernetes-based infrastructure, some teams may struggle to implement GitOps in more complex cloud projects that use a variety of resource types and deployment hosts.

In this article, we'll explore why GitOps is still relevant for these complex cloud projects, and how teams can implement GitOps practices even when using a variety of resource types and deployment hosts.

# How is GitOps different from Continuous Deployment

GitOps is a practice that extends the principles of Continuous Deployment, where CD is focused mostly on application code and how to continuously deploy the always in deployable state main branch of Git to production, GitOps also keeps, monitors and deploys infrastructure.

# Why we keep the Git in the GitOps name?

This Continuous Deployment practice is different from other Operations practice in focusing on Git as the only source of truth, for _infrastructure_ and _application code_. Having the infrastructure as code beside the application code, the practice is focused on syncing the production environment with the changes that occur in the Git repositories using automation. All that Git centric approach is the reason for using the name. Initially can be seen as redundant, as practically the whole industry is using Git on one or several of its flavours as repository for infrastructure and code, but with the name, we can distinguish this ops from other ops.

# Do I need Kubernetes to implement GitOps?

No, you do not need Kubernetes to implement GitOps. While Kubernetes and its ecosystem of tools like ArgoCD have become popular for GitOps implementations, GitOps is a methodology that can be applied to any type of infrastructure and deployment pipeline.

GitOps is all about using Git as the single source of truth for both application code and infrastructure code. With GitOps, any changes to code or infrastructure are made by committing to Git, and then an automated pipeline deploys those changes to the target environment. The automation and monitoring of these changes is also managed through Git.

While Kubernetes is a popular infrastructure choice for many organizations, it is not the only one. GitOps can be implemented on a wide variety of infrastructure types, including cloud providers like AWS, Azure, and Google Cloud, as well as on-premises data centres.

In fact, some organizations may find that Kubernetes is not a good fit for their infrastructure needs, and may choose to use other tools instead. For example, serverless architectures may not require a Kubernetes cluster, and instead can be managed using a tool like AWS Lambda or Azure Functions.

GitOps can be implemented for complex cloud architectures that involve a combination of infrastructure types, such as Kubernetes clusters, serverless infrastructure, and virtual machines. While Kubernetes is often the focus of GitOps discussions and tooling, it's important to remember that it is just a part of the overall architecture. GitOps can still be applied to the entire system, but with external tools that can manage and monitor the infrastructure and application code across different hosting platforms. This allows for a unified approach to deployment, regardless of the underlying infrastructure.

The key to implementing GitOps is to have a well-defined deployment pipeline that is integrated with Git, and that can automate the deployment of changes to the target environment. This pipeline should also have robust monitoring and alerting capabilities, so that any issues can be quickly detected and resolved.

In summary, while Kubernetes and its ecosystem of tools have become synonymous with GitOps, it is important to remember that GitOps is a methodology that can be applied to any type of infrastructure and deployment pipeline. The key is to use Git as the single source of truth, and to have a well-defined automated deployment pipeline that integrates with Git.
