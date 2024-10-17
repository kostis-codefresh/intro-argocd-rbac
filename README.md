# Securing Argo CD in a Multi-Tenant Environment with Application Projects

Let’s take a look at a full example. In our imaginary company, we have 2 developer teams (A and B) that continuously deploy applications. We also have infrastructure applications (i.e., cert-manager) handled by the operator team.

Here are our requirements:

* Admin/operator can view/edit all applications (including infra apps).
* Team B can only view/edit their own applications and nothing else.
* Team A can view/edit their own applications and view-only applications from team B.
* No developer from either team can view the infrastructure applications.
* No developer can delete any application (even their own).
* All applications (including infra) can only be synced from a specific GitHub organization/user.

Read the full blog at https://codefresh.io/blog/multi-tenant-argocd-with-application-projects/
