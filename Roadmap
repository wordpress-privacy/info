# Main goal
Add tools to help site owners comply with the GDPR and other privacy laws and requirements.

## Add notices for both registered users and commenters on what data is collected in core by default, and why.

   * Shorter texts in core with links to more information. Needs text.
   * Create these “more information” pages on WordPress.org. Needs text.

## Create some guidelines for plugins on how to get compliant.
A page (or several pages) on WordPress.org. Needs text.

## Add tools to core to facilitate compliance, and privacy in general.
There are few plugins that have started implementing these tools, so we have a nice head start.

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
      
## Add documentation/help for site owners on how to use these tools.
This should probably be another page under the Tools menu and contain short explanation of what privacy tools are available and how to use them. It could also contain the actual tools, for example an input field for anonymizing commenters by email address.
There are a few things that need clarification:

   * IP addresses may be considered personal data so they need to be deleted or anonymized. However do they need to be sent to the user when requesting to see or download their personal data? They are essentially third-party tokens used temporarily to access the Internet and the users have no control over them. Do other websites make them available?
   * Who are considered “controllers”? All admins on single install and all superadmins on multisite? Are admins on multisite controllers for their own site?
