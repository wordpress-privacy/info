# Main goal

We cannot make WordPress sites compliant, but we can provide site administrators and users with the tools they need to help them bring their sites into healthy compliance.

This project works towards the 25 May 2018 deadline, and the constraints and expectations, of GDPR. It does, however, take a wider generalist view of online privacy in general, and considers privacy and data protection issues outside GDPR's explicit scope.

This project has four goals.

## Add tools to core to facilitate compliance, and privacy in general.

This area of work deals with data collection, retention, and user accounts in WordPress core.

All GDPR related tickets in core can be accessed [here](https://core.trac.wordpress.org/query?status=!closed&keywords=~gdpr). All trac tickets being reviewed for this project can be accessed [here](https://github.com/gdpr-compliance/info/blob/master/Trac-Tickets.md).

### User data

This section deals with user rights to view their data, to download it, and to have their data deleted.

A good amount of this functionality already exists. Registered users ("author" and above) have access to almost all of their personal data on the User Profile screen. They also have access to all posts and comments they have made on the site, and can edit or delete them. Site owners can expect to deal mostly with requests from "contributor" level users as well as people that have commented on the site.

A couple of tasks can be performed in core without additional tools. For example, a registered user’s account can be deleted and all of their posts can either be deleted or reassigned to another (already created) user account. This is sufficient for anonymizing a user account if there are no plugins that store private user data outside user_meta. Also, admins can search for and delete a specific user’s comments.

However, having specialized tools will enable plugins to hook into the performed actions and do their share. This is critical as many of the top 100 plugins seem to store at least some private user data. Tools will also support user data requests on larger, more complex sites where manual review of posts and comments would otherwise take a lot of time.

There will be two main tools:

   * A tool to export all personal data stored on the site (by email address or user login), see #43438, #43440, #43547, #43547.
   * A tool to delete all personal data and anonymize published/public content (like posts, comments, etc.), see #43637.

The requests to see, download and delete/anonymize private data have to be with a confirmation (double opt-in) to avoid misuse. One possible solution would be to send a token by email when a user or a commenter has requested access to or deletion/anonymization of their private data. Then they will have to submit that token as a confirmation of their request.
(TBD: shall we make this process automatic or should a site owner perform the action upon receiving the confirmed request?)

   * For commenters. The stored private data is emails and IP addresses, the rest is public.
      + Dialog for requesting to see and download their private data.
        TBD: should that data also contain the public portion?
      + Dialog for requesting deletion/anonymization of the data.
        TBD: Deletion or anonymization? Or both and let the site owner decide?
      + Ask for consensus for storing commenter cookies. This can be a (checked) checkbox under the comments form, something like “Save my name, email and site URL in my browser for next time I post a comment. More information”.
   * For registered users. All of the data stored by default is already visible in the user profile (except IP addresses if they have commented on the site), and most can be edited or deleted from there.
      + Button for downloading their private data, including IP addresses if they have commented. Again, should that also contain the public data?
      + Button for requesting deletion/anonymization of their account.
      
      There are several plugins that are implementing similar tools. 

These tools will require a confirmation of the email of the person that requests an action, see #43443 (first version is already committed). When a confirmed request is received, the site owner will perform the action.

This could be done automatically. However deleting and anonymizing will be non-reversible. In this case it’s better if the site owners perform the actions themselves, after additional confirmation if required.

### Data collection and retention in core by default

   * Shorter texts about what information is collected in core, why, and what options users have, with links to more information. Needs text.
   * Create these “more information” pages on WordPress.org and/or the privacy resource site (see below). Needs text.
   
## Add tools for creating a privacy policy

This area of work addresses GDPR-ready privacy notices.

Site administrators whose sites collect or process data on EU residents will be required to display a privacy notice which uses plain, simple language to clearly explain data flows, retention, and user options.

The goal is to add the functionality to help users generate a privacy notice, using tools which automatically report data collection and retention from the site's installed plugins. 

### Collecting information for the privacy notice

There will be wp_get_privacy_policy_page() helper functions for use in themes, etc.

Another idea is to have a “postbox” shown when editing the policy page. All plugins that collect personal data or set cookies can output some concise information about what they collect and store and why. This information should be phrased for inclusion in the site’s privacy policy.

### Publishing the privacy notice

The idea is to create the functionality for a special page for the privacy policy, [#43435](https://core.trac.wordpress.org/ticket/43435) (initial version of this is already committed), and [#43491](https://core.trac.wordpress.org/ticket/43491). The site owners are able to select an existing page or create a new one. 

The core privacy notice tool will also contain boilerplate text that the site owners can use to create their policies. The text will be used as the default privacy policy and will be inserted in the privacy policy page when a new one is created. See [#43473](https://core.trac.wordpress.org/ticket/43491).

Generating a privacy notice is not an automatic task: the tools/functionality would assemble the required information for manual approval and publishing by the site administrator.

## Create some guidelines for plugins on compliance

This area of work is examining the current plugin developer guidelines as they pertain to privacy and data protection.

It will look at legal requirements ahead of GDPR, for example developing to the Privacy by Design principles, and also at general plugin ecosystem issues, such as not being allowed to say that a privacy plugin will make a site "compliant".

## Add documentation/help for site owners on how to use these tools.

This area of work will provide guidance for site administrators, plugin developers, and everyday users on how use the tools produced by this project. It will also provide general information on privacy and data protection issues, mindful of the need to discuss general best practice principles rather than one specific legal framework.

This information will reside in a new, separate, side blog, currently under construction, and similar to the [Transparency Blog](https://transparency.automattic.com/). 

Documentation could also be supplied under the Tools menu, inclusive of short explanations of what privacy tools are available and how to use them. It could also contain the actual tools, for example an input field for anonymizing commenters by email address.

The documentation should also be available via the new Tools => Privacy screen. 

## Current issues of concern:

* There are few plugins, including Jetpack and WooCommerce, which have begun similar GDPR compliance work, dovetailing neatly with the Core project. Participants should keep an eye on these to avoid duplication of effort.
* There are also various projects underway for non-Automattic plugins, including some independent GDPR compliance projects. It would be helpful if contributors to the latter plugins would participate/contribute in this GDPR project to avoid duplication of effort or miscommunication.
* IP addresses may be considered personal data so they need to be deleted or anonymized. However do they need to be sent to the user when requesting to see or download their personal data? They are essentially third-party tokens used temporarily to access the Internet and the users have no control over them. Do other websites make them available?
* Who are considered “controllers”? All admins on single install and all superadmins on multisite? Are admins on multisite controllers for their own site?
