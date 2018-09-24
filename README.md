# Welcome to IBM Cloud Onboarding
The IBM Cloud can be complex and somewhat overwhelming, but we're here to help you make sense of it.  This is a technically focused set of pages that will allow you to more easily onboard and effectively use the technology, see the latest best practices, and help you master the IBM Cloud.

# Contents
- **[Introduction - Getting Started](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#introduction---getting-started)**
  - [Cloud Basics](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#cloud-basics)
  - [Organization of the Materials](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#organization-of-the-materials)
- **[IBM Cloud Onboarding for Strategists](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#ibm-cloud-onboarding-for-strategists)**
  - [Account types on the IBM Cloud](https://github.com/dtoczala/IBM_Cloud_Onboarding#account-types-on-the-ibm-cloud)
  - [Setting up a Functional ID for your Account Owner](https://github.com/dtoczala/IBM_Cloud_Onboarding#setting-up-a-functional-id-for-your-account-owner-see-admin)
  - [Federation of your IBM Cloud ID's](https://github.com/dtoczala/IBM_Cloud_Onboarding#federation-of-your-ibm-cloud-ids)
  - [Security Models](https://github.com/dtoczala/IBM_Cloud_Onboarding#security-models)
  - [Project types and IBM Cloud Usage](https://github.com/dtoczala/IBM_Cloud_Onboarding#project-types-and-ibm-cloud-usage)
- **[IBM Cloud Onboarding for Administrators](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#ibm-cloud-onboarding-for-administrators)**
  - [Setting up a Functional ID for your Account Owner](https://github.com/dtoczala/IBM_Cloud_Onboarding#setting-up-a-functional-id-for-your-account-owner)
  - [Naming Conventions](https://github.com/dtoczala/IBM_Cloud_Onboarding#naming-conventions)
  - [Administrative Tasks](https://github.com/dtoczala/IBM_Cloud_Onboarding#administrative-tasks)
  - [Suggested Documentation](https://github.com/dtoczala/IBM_Cloud_Onboarding#suggested-documentation)
  - Support ADDME!!!
- **[IBM Cloud Onboarding for Users](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#ibm-cloud-onboarding-for-users)**
  - [How to Get an IBM ID](https://github.com/dtoczala/IBM_Cloud_Onboarding#how-to-get-an-ibm-id)
  - [Choosing Services](https://github.com/dtoczala/IBM_Cloud_Onboarding#choosing-services)
  - [Joining Projects](https://github.com/dtoczala/IBM_Cloud_Onboarding#joining-projects)
  - [Account Context](https://github.com/dtoczala/IBM_Cloud_Onboarding#account-context)
  - [Educational Resources](https://github.com/dtoczala/IBM_Cloud_Onboarding#educational-resources)
  - Support ADDME!!!

---
# Introduction - Getting Started
You want to work on the IBM Cloud - but you want to be smart about what youy are doing.  We're here to help.  This is a collection of best practices and guidance on how to best administer, govern, configure and have your users onboard onto the IBM Cloud.  We're doing this as an open project on GitHub so we can share these practices with the wider community of IBM professionals and our customers.  Please feel free to contact [Daniel "Tox" Toczala](mailto:dtoczala@usibm.com), if you would like to contribute to this project.

The IBM Cloud is rapidly evolving and changing to better meet the needs of our customers.  If you have topics or subjects that you would like to see addressed here, please open an issue for this project, so we can have other community members begin to contribute and address these areas.

## Cloud Basics
The IBM Cloud has two major components, and it is good to have a basic understanding of both.   The first model is based on Cloud Foundry.  The [Cloud Foundry access model](https://console.bluemix.net/docs/iam/cfaccess.html#cfaccess) is a framework for establishing a hierarchy of user access and security roles for an organization.  It is based on a hierarchy of conceptual groupings, with the **Account** at the top, which may have one or more **Organizations** which belong to the **Account**.  Each **Organization** may have one or more **Spaces** which are associated with it.  Each Account/Organization/Space represents a working environment.

The IBM Cloud started out with ONLY the Cloud Foundry model, but now also has support for [IAM (IBM Cloud Identity and Access Management)](https://console.bluemix.net/docs/iam/users_roles.html#userroles) which uses the concept of Resource Groups and Access Groups to provide user access and security controls.  These Resource Groups serve as the “home” for a variety of different infrastructure and IBM Cloud services.  Access to these Resource Groups can be given on an individual basis, or can be assigned through the use of Access Groups.  If you want to learn more about Resource Groups, Access Groups, and the IBM Access Management (IAM) system, read this great paper on [Getting Started with IBM Cloud IAM](https://github.com/jamesbeltonIBM/IBMCloudIAM/blob/master/IBM%20Cloud%20and%20IAM.pdf).

The IBM Cloud documentation has a [diagram of all of these relationships](https://console.bluemix.net/docs/api/content/account/images/account_diagram.svg), and a [brief description of all of these things](https://console.bluemix.net/docs/account/account_overview.html#overview) and how they all interact.  It's worth reading.

### References for Further Reading
- [Signing Up for the IBM Cloud](https://console.bluemix.net/docs/account/adminpublic.html#signing-up-for-ibm-cloud) - Documentation on getting started.
- [Account Hierarchy](https://console.bluemix.net/docs/account/account_overview.html#overview) - The IBM Cloud documentation has a [diagram of all of these relationships](https://console.bluemix.net/docs/api/content/account/images/account_diagram.svg), and a great description of how they all interact.
- [Getting Started Right on the IBM Cloud](https://dtoczala.wordpress.com/2018/09/20/getting-started-right-on-the-ibm-cloud/) - a good primer on getting started with IBM Watson services on the IBM Cloud.
- [IBM Cloud – Identity and Access Management](https://github.com/jamesbeltonIBM/IBMCloudIAM) - An EXCELLENT beginner’s guide to understanding IAM written by [James Belton](https://github.com/jamesbeltonIBM).  My recommendation for the place to start when attempting to understand IAM on IBM Cloud.
- [Bluemix CLI Commands for Managing Keys and Policies](https://console.bluemix.net/docs/cli/reference/bluemix_cli/bx_cli.html#bx_commands_iam) - a listing and description of the various command line options for managing keys and policies for IAM.
- [IAM Recipe for IBM Cloud Access & Migration Path from CF](https://brandymguillory.wordpress.com/2018/05/31/iam-recipe-for-ibm-cloud-access-migration-path-from-cf/) - a nice walk through of setting up IAM for a real-world application.

## Organization of the Materials
We have organized the material here to try to be helpful for the administrators of the IBM Cloud, the strategists using the IBM Cloud, and the developers and technical users of the IBM Cloud.  Each of these groups will have a "section" of this project, and you will see that this is organized around that idea.

# IBM Cloud Onboarding for Strategists

## Account types on the IBM Cloud
Since we are thinking about doing "real" application development work, we're going to need more capability than the trial and free versions of the services provide.  That means that you will need to spend some amount of money to host these various services and capabilities.  Check out this nice overview of the various [IBM Cloud Account Types](https://console.bluemix.net/docs/account/index.html#subscription) to get an idea of your options.  The capabilities and limitations of these options differ, so it is important that you understand them.

Subscription billing can be done in a variety of ways, you should check with your IBM Sales representative for your available options.  Some things to keep in mind when you have a subscription:
- Subscriptions are typically for a set period of time.  You will be expected to have a constant "burn rate", but you should think of your subscription as being something like a pre-paid card.  As you use IBM Cloud services and capabilities, you will burn down the money left on your card.  Whatever you don't use at the end of the subscription period is lost - so don't over-commit on your subscription.
- What happens when I "go over" on my subscription?  When you run out of funds on your subscription, you will begin to incur charges on a pay-as-you-go basis.  This is often referred to as an overage.


It is important to know and understand the distinction between Infrastructure as a Service (IaaS) and Platform as a Service (PaaS).  ***IaaS services*** are commonly found in the ***Infrastructure*** section on the IBM Cloud.  This includes things like [bare metal servers](https://console.bluemix.net/catalog/infrastructure/bare-metal), [virtual servers](https://console.bluemix.net/catalog/infrastructure/virtual-server-group), [VMWare vSphere](https://console.bluemix.net/infrastructure/vmware-solutions/console/gettingstarted/vss), [load balancers](https://console.bluemix.net/catalog/infrastructure/load-balancer-group), [internet services](https://console.bluemix.net/catalog/services/internet-services), and other similar resources.  ***PaaS services*** tend to be everything else, including things like [Blockchain networks](https://console.bluemix.net/developer/blockchain/dashboard), [Databases](https://console.bluemix.net/catalog/services/cloudant), and the [various Watson services](https://console.bluemix.net/developer/watson/dashboard).

When you sign up for the IBM Cloud, you will get a personal account set up, which is associated with your username (typically your email ID).  This account is a trial account - it allows you to do things for free, and to use free plans for most of the services on the IBM Cloud.  This is your **PaaS account**.  if you look at your profile in the upper right hand corner of your browser window, you might see a 7 digit number before your name.  This seven digit number is your ***linked IaaS account***.  This allows you to easily use both IaaS and PaaS resources within the same account - and it is part of our "One Cloud" goal at IBM.  If you do not have a linked account, and you would like one, please contact your IBM team, or open a support ticket asking for the creation of a linked account.

## Setting up a Functional ID for your Account Owner (see Admin)
For more information on setting up a [functional ID for your account owner](https://github.com/dtoczala/IBM_Cloud_Onboarding#setting-up-a-functional-id-for-your-account-owner), see the write up in the Admin section.

## Federation of your IBM Cloud ID's
Federation of your IBM Cloud ID's is important to understand.  When you first get onto the IBM Cloud, you sign up for an account, typically using your corporate email address as your IBM ID.  You then create a password, which is specific to the IBM Cloud.  However, if you Federate your IBM Cloud ID's then you will authenticate against YOUR corporate ID servers, using your own internal ID (corporate email address) and your own corporate password.  This allows you to also set up a [Single-Sign-On (SSO) capability for your IBM Cloud](https://console.bluemix.net/docs/customerportal/cpmanacctconfsso.html#cp_setupsso).

You can learn more about federating your IBM Cloud ID's by reading the [IBMid Enterprise Federation Adoption Guide](https://ibm.ent.box.com/notes/78040808400?v=IBMid-Federation-Guide).  It covers many of the technical details of account federation, as well as an overview of the process.

Once you have federated IBM Cloud ID's, you will be able to more easily manage your users using things like [dynamic rules for access groups](https://console.bluemix.net/docs/iam/accessgroup_rules.html#rules) to do automated access control that is in line with your corporate security guidelines.

## Security models
The IBM Cloud currently operates with two different securoity models, which were mentioned in the [Cloud Basics](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#cloud-basics) section.  Here we will be digging into these two different models in more depth.

### Cloud Foundry Orgs and Spaces
The [Cloud Foundry access model](https://console.bluemix.net/docs/iam/cfaccess.html#cfaccess) is a framework for establishing a hierarchy of user access and security roles for an organization.  It is based on a hierarchy of conceptual groupings, with the **Account** at the top, which may have one or more **Organizations** which belong to the **Account**.  Each **Organization** may have one or more **Spaces** which are associated with it.  Each Account/Organization/Space represents a working environment.

Your users can be assigned one of three different roles at the **Organization** level.  These are:
- Managers - Organization managers can create, view, edit, or delete spaces within the organization, view the organization's usage and quota, invite team members to the Organization, manage who has access to the Organization and their roles in the Organization, and manage custom domains for the Organization.
- Billing Manager - Billing managers can view runtime and service usage information for the organization on the Usage Dashboard page.  Multiple Organizations can often have the same Billing Manager.
- Auditor - Organization auditors can view application and service content in the organization. Auditors can also view the team members in the Organization and their assigned roles, and the quota for the Organization. This role is assigned to all invitees by default.

Your users can be assigned one of three different roles at the **Space** level.  These are:
- Manager -   Space managers can add existing team members and manage roles within the Space. The Space manager can also view the number of instances, service bindings, and resource use for each application in the space.
- Developer –  Space developers create, delete, and manage applications and services within the Space. Managing tasks include deploying apps, starting or stopping apps, binding or unbinding a service to an application. The Space developer can associate internal or external URLs with an application in the space.
- Auditor -  Space auditors have read-only access to all information about the space, such as information about the number of instances, service bindings, and resource use for each application in the Space.

The combination of the two roles, at the organization level and at the space level, will control what your users can and cannot do in the various spaces on the IBM Cloud.

### Resource Groups and Access Groups
The IBM Cloud started out with ONLY the Cloud Foundry model, but now also has support for a [IAM (IBM Cloud Identity and Access Management)](https://console.bluemix.net/docs/iam/users_roles.html#userroles) which uses the concept of Resource Groups and Access Groups to provide user access and security controls.

Resource Groups can be thought of as being similar to spaces - thety are where a set of services "live", and they determine the ability of users to see and access those services.  There are two major differences between these two: 1) resource groups do not live in a hierarchy like spaces do; and 2) the security model is different (and quite a bit more granular).

Let's examine the [IAM security model](https://console.bluemix.net/docs/iam/users_roles.html#userroles) in a little more depth.  The account owner or administrator will be able to assign policies for both the platform management roles and the individual service roles.  Platform management roles deal with overall resource group permissions, roles and access capability.  You can assign platform managment roles at four different levels:

- **Viewer role** - in this role you can view instances, aliases, bindings, and credentials for the resource group.
- **Operator role** - in this role you can view instances aliases, bindings, and credentials for the resource group, and you can also manage all of these.
- **Editor role** - in this role you can view and manage instances aliases, bindings, and credentials for the resource group.  You can also rceate, delete, edit, and view service instances.
- **Administrator** role - in this role you can do ALL management actions within the resource group

In addition to the platform managemnt roles, you can also assign roles and policies for each specific service. Most services will have a simple core of three policies (Manager, Reader, Writer) - but individual services can implement policies and  
roles that are unique for them.  You will need to check the documentation for a particular service to know (and then assign) proper roles and policies for each service.

## Project types and IBM Cloud Usage

### Internal Projects

Internal projects are easy.  You don't need to worry about passing along costs to end customers, and you shouldn't have to worry too much about the visibility of the charges being generated on the IBM Cloud.  All you need to make sure of is that you are following adequate [Naming Conventions](https://github.com/dtoczala/IBM_Cloud_Onboarding#naming-conventions), so you can properly do any chargebacks and calculate costs to the business.

### External Projects

You need to be aware of your business model, and specifically how you anticipate deploying and generating revenue from your application.  If your application is being provided to your customers as a convenience, or as part of a larger capability, then you don't have to worry about passing along the costs of your IBM Cloud based capabilities.  That makes it very much like an internal project - you just need to track and isolate the costs.

If your application is provided to customers as a capability and you would like to pass along the charges incurred, then you will need to figure out how to implement this business model.  There is nothing built into the IBM Cloud capabilities that differentiates between API calls, or some of the other usage/billing metrics.  Your application will need to track customer specific usage of the various IBM Cloud capabilities, and then provide a way to trace this usage back to the charges incurred on the IBM Cloud platform.  This can be difficult to maintain, as API's change and pricing changes over time.  

We much more strongly recommend that our customers provide capability in tiers to their customers, and that they then try to recover their IBM Cloud costs in a less granular manner.  So your organization will be charging customers a monthly fee based on usage, perhaps across three tiers (light, medium, heavy), and then having the sum of all of these user fees roughly cover the monthly IBM Cloud costs.  This will be easier to maintain, and will require less operational overhead in the long run.

# IBM Cloud Onboarding for Administrators
IBM Cloud Administrators can face different challenges and will have different concerns that other user groups.  Sometimes the IBM Cloud Administrator will be a 

## Setting up a Functional ID for your Account Owner
When looking to use the IBM Cloud for organizational (or Enterprise) use, it is considered a best practice to have your organization procure an IBM Cloud subscription (see the section on [Account types on the IBM Cloud](https://github.com/dtoczala/IBM_Cloud_Onboarding#account-types-on-the-ibm-cloud)).  Your subscription should be associated with an organization email address, not a personal user address.  This means that you will need to ask your IT department for a functional email address (or Functional ID) that is not associated with any one user.  This will be your IBM Cloud Administrator account.
This is done because often people change roles within a company, or leave a company, and accessing their account once this happens could be difficult (or impossible).  You don't want your organizational cloud infrastructure with a single point of failure.
For example, if I was setting up an IBM Cloud account and environment for the Acme company, I would not associate the account with my email address (joe.smith@acme.com).  Instead, I would have an new email account created called IBMCloudAdmin@acme.com, and I would use this account to create a new IBM Cloud account ID, and then use this ID for all IBM Cloud administrative activities.
Keep in mind that this new account should be auto-forwarding email to a small group of people within your organization.  The IBM Cloud team will sometimes email updates on critical issues and maintenance activites to the owner email address, and you want to make sure that ALL of your administrators see these emails.

## Naming Conventions

A failure to use naming conventions for your orgs, spaces, and resource groups, will lead to increased administrative burden, and the confusion of your Cloud users.  Solid naming convetions will make chargebacks easier to compute, and will help your users (both technical and non-technical) to more easily navigate all of the projects in flight on the IBM Cloud.

Below is a set of naming conventions that we have used in many different environments.  Feel free to use these as-is, or to make modifications to them.  The important thing is that you establish naming conventions, and that you remain consistent in following those conventions.

- **Organizations** -   **<project_name>_ORG**
    - For example, AlphaProj_ORG.
- **Spaces** - **<project_name>_\<environment>_SPC**
    - For example, AlphaProj_Dev and AlphaProj_Test spaces.  Try to have a common set of environments: like Dev, Test, QA, Staging, Pre-Prod, etc.
- **Resource Groups** - **<project_name>_\<environment>_RG**
    - For example, AlphaProj_Dev_RG and AlphaProj_Test_RG groups (which are paired with the corresponding spaces).
- **Access Groups** - **<project_name>_\<environment>_\<usertype>_AG**
    - For example, AlphaProj_Dev_Devs_AG and AlphaProj_Test_Admins_AG access groups.  Try to have a common set of user types: like Devs, Testers, Admins, DBAs, Architects, etc.

## Administrative tasks
Talk about how you want to script as much as possible.

### Adding new users

### Adding new projects

### Billing and billing issues

### Removing Users

### Archiving Projects

## Suggested Documentation
What things should you be maintaining (documents, dashboards, etc.) to communicate the state of everything going on inside your IBM Cloud area?

## Training Available
There is not a lot of training available that is focused on IBM Cloud administration right now.  One option that you have is to follow the [Learning Journeys](), and go and look at the following two learning journeys:
- [Administering a Cloud Infrastructure](https://www-03.ibm.com/services/learning/itesp.wss/zz-en?pageType=journey_description&journeyId=LDE-ITNS_189) - primarily focused on Softlayer (IaaS or Infrastructure as a Service) administration.  This is older, so the user interfaces have changed a bit, but the basic concepts still hold true.
- [Administering a Bluemix Based Application](https://www-03.ibm.com/services/learning/ites.wss/zz-en?pageType=journey_description&journeyId=adblmx_1) - this content is older (Bluemix is the former name of the IBM Cloud), so the user interfac e will be different, but most of the concepts still hold true.

# IBM Cloud Onboarding for Users
Getting onto the [IBM Cloud is easy](https://console.bluemix.net), and beginning to use the services and capabilities of the IBM Cloud is relatively easy as well.  It's important that you understand the basic cloud concepts from the [Introduction - Getting Started](https://github.com/dtoczala/IBM_Cloud_Onboarding/tree/master#introduction---getting-started) section.  Make sure that you review that section.

## How to get an IBM ID
If your company or organization has an existing IBM Cloud subscription, and they have federated IBM Cloud ID's, then all you need to do is to go to your [IBM Cloud dashboard](https://console.bluemix.net/dashboard/apps), and supply your corporate ID (typically an email address like joe.smith@acme.com) and your corporate password.  When a company decides to federate the ID's of it's users, those users authenticate against their own's company's identity servers, and everyone with a valid corporate ID will have access to the IBM Cloud.
if you are not lucky enough to work with a company with federated ID's, you will need to go out and [create an IBM Cloud account](https://console.bluemix.net/registration/) for yourself.  We suggest making your login the same as your corporate email address.  This means that you'll be able to maintain your account in the future, if your company decides to federate ID's in the future.  Supply the information asked for, and make note of your password, and you will be all set.

## Choosing services


### Choosing service plans

### Using Service Credentials

### Learning about services

## Joining projects

## Account context 
"Why can't I see the services that I created yesterday???"

## Educational Resources
There is specialized support and training for all of the services on the IBM Cloud.  When looking at the service in the catalog, just click on the **View Docs** link, and you will see not only service documentation, but starter projects, and other materials to help you get started with that particular service.

There is also a more general course, called [Administering a Bluemix Based Application](https://www-03.ibm.com/services/learning/ites.wss/zz-en?pageType=journey_description&journeyId=adblmx_1), but this content is older (Bluemix is the former name of the IBM Cloud).  The user interface will be different, but most of the concepts still hold true.
