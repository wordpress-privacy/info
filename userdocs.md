# User Privacy and your WordPress site

Depending on the national or international privacy regulations, such as the EU's General Data Protection Regulation, which may be applicable to you, you may be required to display a privacy policy disclosing your collection and sharing of personal data. You may also be required to provide your users with the means to request a copy of the information you hold about them, or request its deletion.

WordPress now includes simple tools for site administrators to take these steps. These tools make it easier for you to inform your users, through a transparent privacy notice, what data you collect about them, why, and how; what you do with that data, including who you share it with. They also make it easier for users to request a copy of their data or its removal. The use of these tools, whether required by law or not, will make it easier for you to protect your users' privacy.

Every website is different. No two privacy notices will be alike, just as no two site administrators will have identical compliance journeys. Additionally, new regulations, as well as adaptations of existing ones, may alter your compliance journeys. **We strongly encourage you to consider that safeguarding privacy is not a one-time responsibility.** Taking steps to secure and protect your users' data is a continuous process both online and offline. These tools can help you with parts of that process, but they are not a compliance process in and of itself. *We strongly encourage you to check the regulations and expectations applicable to you and adjust your usage of these tools as needed.*

## Privacy Settings

This tool makes it easier to select and build a Privacy Policy page. It will create a dedicated page, or adapt an existing one, and provide prompts and headers to kickstart the process.

Site administrators can create this page by going to  *Settings > Privacy*, Where the Privacy Policy page manager will be used. 

The prompts and headers provided in the tool by default are based on the expectations of Europe's GDPR as a leading privacy standard. While this gives you a start to build on, your privacy policy is not constrained by this starter text. *It is your responsibility* to write a comprehensive privacy policy, to ensure that it reflects all national and international legal requirements on privacy, and to keep your policy current and accurate. 

### Privacy Policy Editing Helper

The *Editing Helper* feature is part of the new *Privacy Settings* tool. Drawing information from both WordPress core and a site's themes and plugins, the Editing Helper pulls together a collected set of default texts which detail a site's data collection and sharing, generating a starter text which you can use to complete your privacy policy.

While you do not necessarily need to use this tool to build a Privacy Policy, we believe it is helpful because it provides information on how your WordPress site collects and processes data in both core and plugins. It is important to consider these back-end uses of data. While not all sites will use all functions - for example, an administrator may choose not to enable comments on posts - nearly every site uses features such as analytics cookies, social media sharing buttons, or contact form plugins. Please add as many additional disclosures as is necessary to be fully transparent about how your site uses personal data.

Additionally, many sites will embed third party tools, such as email subscription services, which collect data in ways the the Editing Helper tool cannot detect, so the default template may not completely describe how your site might collect data about its user. Take the time to understand how these functions collect user data, and use your policy to describe what a user should know. 

Theme and plugin developers are invited to learn how the Privacy Policy Editing Helper works, and to feed in the information about how your theme or plugin collects data into the privacy policy tool.

## Export Personal Data tool

WordPress now includes a feature to to archive user data for export. This is different from the _Tools > Export_ tool which creates an archive file of posts, pages, or media; the new tool exports infomration captured elsewhere. You can use this tool by clicking on _Tools > Export Personal Data_ in your WordPress dashboard. 

This tool manages email export requests by your users. Following manual approval, it allows you to generate a (`.zip` format) file containing the personal data which exists about a user within your WordPress site. 

*We strongly encourage you use the email validation feature built into the export tools. This confirmation process will help safeguard against abuse, such as malicious users pretending to be someone they are not.*

While this tool's scope covers much of the scope of WordPress user data, it likely does not include information that may be collected by your site using a third party, such as an analytics provider, newsletter subscription service, ad affiliate partner or embedded media. So while the tool can give you a good start in providing your users with the data they have requested, every site administrator should understand what data they collect and process outside their WordPress site.

## Erase Personal Data tool

Similar to the Export Personal Data tool, WordPress now includes a tool to delete a user's personal data upon verified request. You will find this feature under _Tools > Erase Personal Data_ in your WordPress dashboard.  

As with the Export tool, the Erase Personal Data tool uses email validation to send a user's request to an administrator. The administrator must manually approve the request to remove the data in question. *We strongly encourage you use the email validation feature built into the export tool. This confirmation process will help safeguard against abuse, such as malicious users pretending to be someone they are not.*

Erasure requests cannot be reversed after they have been confirmed. *Deleted data is permanently removed from the database.* It does not remove the data from backups or archive files. When using the tool alongside automated backups or archives, we advise you to exercise caution when restoring user data from backups. When restoring an archived copy of your site, your requests for erasure should be respected.

As with the Export tool, while this tool's scope covers much of the scope of WordPress user data, it likely does not include information that may be collected by your site using a third party, such as an analytics provider, newsletter subscription service, ad affiliate partner or embedded media. So while the tool can give you a good start in providing your users with the data they have requested, every site administrator should understand what data they collect and process outside their WordPress site.

It is also important to understand that personal data deletion requests are not absolute. A site administrator is not obliged to delete data that they may be required to keep for other legal or statutory reasons. For example, you may be required to keep sales records for a certain number of years for tax purposes. You may also wish to keep a user's records for security purposes, for example, if there is an ongoing investigation into abuse. These situations should be handled internally.

## Explicit Consent (Can we take this out if we have nothing to show for it?)
Under some privacy laws, you may also be required to have your users' explicit consent before collecting their personal data. While WordPress.org does not yet have some of these tools built, [there are various plugins available](https://wordpress.org/plugins/tags/gdpr/) to help in collecting consent. Other plugins, especially in the case of forms, suggest that you add a "required" consent field that says something like [_"I consent to my submitted data being collected and stored"_](https://docs.gravityforms.com/wordpress-gravity-forms-and-gdpr-compliance/
) if this is a requirement for your website.
***
To-do:
Would be nice if we could add a "how-to-use" section - see Woo article here doing a good job: 
https://woocommerce.wordpress.com/2018/05/04/woocommerce-3-4-gdpr-features/
