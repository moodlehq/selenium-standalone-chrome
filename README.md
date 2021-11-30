# selenium-standalone-chrome

This repository contains build files for a custom version of the official selenium/standalone-chrome docker image.

It includes a copy of chromedriver which includes certain bug fixes, which have already been merged into later versions of the Chromoium project.

## Tags available
The following tags are currently available:

| Tag                        | chromedriver version | Selenium version              | Bugs addressed | Architectures |
| -------------------------- | -------------------- | ----------------------------- | -------------- | ------------- |
| 3.141.59-20210929-moodlehq | 94.0.4604.0          | 3.141.59, revision e82be7d358 | zerosize       | amd64         |

## Bugs addressed

### Zero Size issue for items close to edge of viewport (zerosize)
This issue was discovered by MoodleHQ, reproduced, reported, and fixed using the following patch:
https://chromium-review.googlesource.com/c/chromium/src/+/3088886

The original bug report is available at https://bugs.chromium.org/p/chromedriver/issues/detail?id=3878
