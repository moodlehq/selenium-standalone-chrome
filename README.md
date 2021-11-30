# selenium-standalone-chrome

This repository contains build files for a custom versio of the official selenium/standalone-chrome docker image.

It includes a copy of chromedriver which includes certain bug fixes, which have already been merged into later versions of the Chromoium project.

## Tags available
The following tags are currently available:

| Tag                        | chromedriver version | Selenium version              | Bugs addressed       | Architectures |
| -------------------------- | -------------------- | ----------------------------- | --------------       | ------------- |
| 96.0-moodlehq              | 96.0.4664.45         | 4.1.0 revision 87802e897b     | zerosize, decoration | amd64         |

## Bugs addressed

### Zero Size issue for items close to edge of viewport (zerosize)
This issue was discovered by MoodleHQ, reproduced, reported, and fixed using the following patch:
https://chromium-review.googlesource.com/c/chromium/src/+/3088886

The original bug report is available at https://bugs.chromium.org/p/chromedriver/issues/detail?id=3878

### Window decoration is not considered when scrolling into view
This issue was discovered, reproduced, and reported by Moodle HQ.
https://chromium-review.googlesource.com/c/chromium/src/+/3281973

It was fixed upstream in Chromedriver version 98.

The original bug report is available at https://bugs.chromium.org/p/chromedriver/issues/detail?id=3933
