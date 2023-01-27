---
title: Meeting Minutes
hide_sidebar: true
---

You can add meeting minutes to a markdown file using the shortcode:
**{{&lt; meeting_minutes &gt;}}**

{{< grid/div class="alert alert-warning" isMarkdown="false" >}} This is for
demonstration only. The only link which is expected to work is under the
Specification Committee tab. {{</ grid/div >}}

{{< meeting_minutes >}}

## Setup

To add meeting minutes, create a **meeting_minutes.yml** file in the data
folder. The YAML file should have a similar shape to the following:

```
dir: '/path/to/directory/with/committees/'
yearly_sections_enabled: true
order:
  - specification_committee
  - marketing_committee
items:
    marketing_committee:
        - title: August 18, 2022 (pdf)
          url: marketing_committee/2022-08-18-marketing-minutes.pdf
          year: 2022
    specification_committee:
        - title: June 28, 2018 (pdf)
          url: https://jakarta.ee/about/meeting_minutes/steering_committee/2018-06-28-specification-minutes.pdf
          year: 2018
```

#### Properties

| Property                  | Description                                                                                                                                                                      |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `dir`                     | is the directory for which to search for the meeting minutes.                                                                                                                    |
| `yearly_sections_enabled` | splits meeting minutes into yearly sections if set to `true`.                                                                                                                    |
| `order`                   | modifies the order of the tabs. It needs to be an array of committee names corresponding to their key under `items`. If this is not set, the tabs will be alphabetically sorted. |
| `items`                   | contains the committees such as `marketing_committee` and `specification_committee`. You can give the committee any key. This committee will appear as a tab on the component.   |
| `title`                   | is the link text of a meeting minutes item.                                                                                                                                      |
| `url`                     | locates the meeting minute file. If `dir` was set, it will locate the file from `dir`.                                                                                           |
| `year`                    | is the year which the meeting was taken. This will dictate which year-section the item will appear under. This is not required if `yearly_sections_enabled` is set to `false`.   |
