# User Privacy and your WordPress site

Depending on your national or international privacy regulations (such as the European Union's General Data Protection Regulationm which may be applicable to you) you may be required to display a privacy policy disclosing your collection and sharing of personal data. Personal data includes things like your users' name, email, birthdate, phone number, IP address and other data that can be used to identify them.

You may also be required to provide your users with the means to request a copy of the information you hold about them, or request its deletion.

WordPress now includes several simple tools for site administrators to take these steps. These tools make it easier for you to inform your users through a transparent privacy notice about data that is collected on your site. It usually includes at least:
- What data you collect about them,
- Why and how you collect data,
- And what you do with that data (including with whom who you might share that data). 

These new tools also make it easier for users to request a copy of their data or its removal. The use of the new data privacy tools (whether required by law or not) will make it easier for you to protect your users' privacy.

Please note: Every website is different. No two privacy notices will be alike, just as no two site administrators will have identical compliance journeys. Additionally, new regulations, as well as adaptations of existing ones, may alter your compliance journeys. **We strongly encourage you to consider that safeguarding privacy is not a one-time responsibility.** Taking steps to secure and protect your users' data is a continuous process both online and offline. These tools can help you with parts of that process, but they are not a compliance process in and of itself. *We strongly encourage you to check the regulations and expectations applicable to you and adjust your usage of these tools as needed.*

## Privacy Settings

This tool makes it easier to select and build a Privacy Policy page. It will create a dedicated page (or adapt an existing one) and provide prompts and headers to kickstart the process.

Site administrators can create this page by going to  *Settings > Privacy*, where the Privacy Policy page setting is managed.

The prompts and headers provided in the tool by default are based on the expectations of Europe's GDPR as a leading privacy standard. While this gives you a start to build on, your privacy policy is not constrained by this starter text. *It is your responsibility* to write a comprehensive privacy policy, to ensure that it reflects all national and international legal requirements on privacy, and to keep your policy current and accurate. 

### Privacy Policy Editing Helper

The *Editing Helper* feature is part of the new *Privacy Settings* tool. Drawing information from both WordPress core and a site's themes and plugins, the Editing Helper pulls together a collected set of default texts which detail a site's data collection and sharing, generating a starter text which you can use to complete your privacy policy.

While you do not necessarily need to use this tool to build a Privacy Policy, we believe it is helpful because it provides information on how your WordPress site likely collects and processes data in core, theme and plugin code. It is important to consider these back-end uses of data: While not all sites will use all functions (for example, an administrator may choose not to enable comments on posts) nearly every site uses features such as analytics cookies, social media sharing buttons, or contact form plugins. Please add as many additional disclosures as is necessary to be fully transparent about how your site uses personal data.

*This tool ONLY collects policy help texts from WordPress and participating plugins.* Many sites will also embed third-party tools (such as email subscription services) which collect data in ways the the Editing Helper tool cannot detect, so the default template may not completely describe how your site might collect data about its user. Take the time to understand how your website actually collects your users' data, and be transparent about what actually happens with data on your website to your users.

Further, theme and plugin developers are invited to learn how the Privacy Policy Editing Helper works, and to feed in the information about how your theme or plugin collects data into the privacy policy tool.

## Export Personal Data tool

WordPress now includes a feature to to archive user data for export. This is different from the _Tools > Export_ tool which creates an archive file of posts, pages, or media; the new tool exports in captured elsewhere. You can use this tool by clicking on _Tools > Export Personal Data_ in your WordPress dashboard. 

This tool manages email export requests by your users. Following manual approval, it allows you to generate a (`.zip` format) file containing the personal data which exists about a user within your WordPress site. 

*We strongly encourage you use the email validation feature built into the export tools. This confirmation process will help safeguard against abuse, such as malicious users pretending to be someone they are not.* As with the Erasure tool, the Erase Personal Data tool uses email validation to send a user's request to an administrator. The administrator must manually approve the request to send the data in question to the user.

*As this tool ONLY gathers data from WordPress and participating plugins, you may need to go beyond to comply with export requests.* While it may give you a good start in providing your users with the information they have requested, every site administrator should understand what data they collect and process outside their WordPress site as a full site request may have more responsibility than simply using this export alone. 

While this tool's scope covers much of the scope of WordPress user data, it likely does not include information that may be collected by your site using a third-party service, such as an analytics provider, newsletter subscription service, ad affiliate partner or embedded media.

## Erase Personal Data tool

Similar to the Export Personal Data tool, WordPress now includes a tool to delete a user's personal data upon verified request. You will find this feature under _Tools > Erase Personal Data_ in your WordPress dashboard.  

*We strongly encourage you use the email validation feature built into the export tool. This confirmation process will help safeguard against abuse, such as malicious users pretending to be someone they are not.* As with the Export tool, the Erase Personal Data tool uses email validation to send a user's request to an administrator. The administrator must manually approve the request to remove the data in question.

*Deleted data is permanently removed from the database.* Erasure requests cannot be reversed after they have been confirmed. Note that it does not remove the data from backups or archive files: When using the tool alongside automated backups or archives, we advise you to exercise caution when restoring user data from backups. When restoring an archived copy of your site, your requests for erasure should be respected.

*As this tool ONLY gathers data from WordPress and participating plugins, you may need to go beyond to comply with erasure requests.* While it may give you a good start in complying with your users' request to remvoe the information they have requested, every site administrator should understand what data they collect and process outside their WordPress site as a full site erasure request may have more responsibility than simply using this tool alone.

In particular (as with the Export tool) it likely does not include information that may be collected by your site using a third-party service, such as an analytics provider, newsletter subscription service, ad affiliate partner or embedded media.

*When erasing user data, this tool does not automatically delete registered users and their profile data.* Administrators should perform that step themselves after successfully erasing personal data for a registered user. User deletion is available for each user in the _Users_ menu in the Dashboard.

*It is also important to understand that personal data deletion requests are not absolute.* A site administrator is not obliged to delete data that they may be required to keep for other legal or statutory reasons. For example, you may be required to keep sales records for a certain number of years for tax purposes. You may also wish to keep a user's records for security purposes, for example, if there is an ongoing investigation into abuse. These situations should be handled internally.

## Explicit Consent 
Under some privacy laws, you may also be required to have your users' explicit consent before collecting their personal data. Further, you may also be required to have your users' "explicit consent" before certain kinds of processing of personal data, if that processing isn't otherwise necessary for your site.

While WordPress.org does not yet have consent tools built, [there are various plugins available](https://wordpress.org/plugins/tags/gdpr/) to help in collecting consent to be compliant with the May 2018 GDPR compliance deadline. In addition, WordPress Core intends to add additional tools for WordPress theme and plugin developers for explicit consent management in WordPress Sites.

Some plugins, especially in the case of forms and email subscription services, suggest that you add a "required" consent field that says something like [_"I consent to my submitted data being collected and stored"_](https://docs.gravityforms.com/wordpress-gravity-forms-and-gdpr-compliance/
) if this is a requirement for your website.

***
_Props to @allendav, @webdevlaw for help here._

Various notes: 

1) To-do: Would be nice if we could add a "how-to-use" section by May 25 launch, see Woo article here doing a good job of this: 
https://woocommerce.wordpress.com/2018/05/04/woocommerce-3-4-gdpr-features/

2) Note: Leaving in "Explicit Consent" even though we don't have much to show for it since it's pragmatically a major concern for major plugins. We should replace with content about WP core when we can.

3) Would like feedback on whether to use link one or two:
- wordpress.org/plugins/tags/gdpr
- https://wordpress.org/plugins/gdpr/
Link two is built by a well-respected development shop and does Explicit Consent the way it should be, but link one is less endorsement-heavy.
