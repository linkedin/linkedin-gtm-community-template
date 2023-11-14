# LinkedIn Insight Tag 2.0 GTM template

This tag template provides LinkedIn’s InsightTag 2.0 implementation for tracking via Google tag Manager’s [Community template gallery](https://developers.google.com/tag-platform/tag-manager/templates/gallery)

## Submitting this template

1.  Sign in to a GitHub with an account that has access to this template repository you wish to add to the Gallery.
2.  Go to the Community Template Gallery at [tagmanager.google.com/gallery](https://tagmanager.google.com/gallery).
3.  Click vertical dots option and select **Submit Template**.
4.  Provide this **Repository URL** in the field provided and click **Submit**.

## Updating this template

### Development

To make changes to the template, follow these steps:

1. Open your Google Tag Manager account and [create a web container](https://support.google.com/tagmanager/answer/12974036?hl=en).
2. [Import](https://developers.google.com/tag-platform/tag-manager/templates#export_and_import) the `template.tpl` file in this repository into the template editor.
3. The template will load into the editor. Make any necessary changes.
4. Once you're done, [export](https://developers.google.com/tag-platform/tag-manager/templates#export_and_import) the template from the editor.
5. Replace the contents of the `template.tpl` file with the contents of the newly generated `.tpl` file.
6. Submit the pull request with the changes.

**NOTE**: Always use the GTM template editor to make updates, _do not_ edit the `template.tpl` file by hand.

### Deployment

The `metadata.yaml` file is used to determine which version of the template to use in the gallery. To publish new versions, we need to add the change number (SHA number) to the `versions` section of the `metadata.yaml` file.

1.  Locate the commit that includes the changes that you want to push, and copy the SHA number. An easy way to do this is in GitHub is to go to a [commit view](https://help.github.com/en/articles/differences-between-commit-views) and click the clipboard icon. This will copy the entire SHA number to your clipboard.
2.  Add a new `sha` entry to the top of your `versions` list in `metadata.yaml`. (See the example below.)
3.  Add `changeNotes` to briefly describe changes contained in this new version. You can create multiline comments, if desired. (See the example below.)
4.  Commit the change to `metadata.yaml` and your update will appear in the gallery typically within 2 to 3 days.

This example demonstrates how to add new version information including the SHA number and change notes:

```
homepage: "https://www.linkedin.com/campaignmanager"
documentation: "https://www.linkedin.com/help/lms/answer/a416960"
versions:
  # Latest version
  - sha: 5f02a788b90ae804f86b04aa24af8937e567874c
    changeNotes: |2
      Fix bug with the whatsamajig.
      Improve menu options.
      Update API calls.
  # Older versions
  - sha: 5f02a788b90ae804f86b04aa24af8937e567874b
    changeNotes: Adds eject button.
  - sha: 5f02a788b90ae804f86b04aa24af8937e567874a
    changeNotes: Initial release.
```

Monitor the status page to ensure the commit has landed: https://tagmanager.google.com/gallery/#/template/linkedin/linkedin-gtm-community-template/status.

Template users will be notified if there is an update to the template and will have the option to [update the template to the latest version](https://support.google.com/tagmanager/answer/9454109#update).
