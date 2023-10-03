# Mild Blue

[![Mild Blue About](https://github.com/mild-blue/about/blob/master/images/assets/readme_about.jpg?raw=true)](https://jobs.mild.blue/)

# About

Information about us, our projects that will be presented anywhere. Mostly in JSON format..

# UI
This app is rendered by [Web presentation](https://github.com/mild-blue/project-web-presentation/)

## Social links settings

Format:

```
"social": [
    {
      "icon": "facebook-f",
      "url": "https://www.facebook.com/mildblueai"
    }
]
```

`icon` - Font Awesome icon name (see [available icons](https://fontawesome.com/icons?d=gallery&m=free)). Icon name is
also used in `class` property on FE for additional styling.
`url` - Link to social media.

## Onepager settings

Settings for [Mild Blue Onepager](https://mild-blue.github.io/onepager/)
. [GitHub repository](https://github.com/mild-blue/onepager/).

Example of settings object:

```json
{
  "team": [
    "tomas",
    "honza",
    "marek",
    "lukas",
    "nasta",
    "beta"
  ],
  "projects": [
    "breviary",
    "txm",
    "datavid",
    "ekg"
  ],
  "showCooperation": false,
  "showSubtitle": true,
  "showCoFounderLabel": true,
  "footerLinkType": "web"
}
```

Attribute | Type | Possible values                                          | Description
--- | --- |----------------------------------------------------------| ---
`team` | `string[]` | `["tomas", "honza", ... (see "people/sources.json")]`    | Team members to be displayed in onepager. Every listed team member has to have their config file in [people directory](https://github.com/mild-blue/about/tree/master/people)
`projects` | `string[]` | `["breviary", "txm", ... (see "projects/sources.json")]` | Projects to be displayed in onepager. Every listed project has to have its config file in [projects directory](https://github.com/mild-blue/about/tree/master/projects)
`showCooperation` | `boolean` | `true` &#124; `false`                                    | Defines whether to render last project block as a block about cooperation with Edwards Lifesciences
`showSubtitle` | `boolean` | `true` &#124; `false`                                    | Defines whether to display submotto (small text next to the logo on the right side of the onepager)
`showCoFounderLabel` | `boolean` | `true` &#124; `false`                                    | Defines whether to display "co-founder" title under co-founders' names.
`footerLinkType` | `string` | `"email"` &#124; `"web"`                                 | If value is set to `email` a link to company e-mail will be shown. If value is set to `web`, link to [mild.blue](https://mild.blue/) web will be shown. Every link type has its corresponding label.


# Development

When creating a PR you can check how the website will look like with your PR by going to https://mild-blue.pages.dev/?source=branch where instead of "branch" fill in the name of your branch.
