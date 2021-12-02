FROM selenium/standalone-chrome:3.141.59

ARG CHROME_VERSION="96.0.4664.45"
ARG DEBVERSION="1"

USER root
COPY chromedriver /opt/selenium/chromedriver-${CHROME_VERSION}-moodlehq
RUN rm /usr/bin/chromedriver && \
    ln -s /opt/selenium/chromedriver-${CHROME_VERSION}-moodlehq /usr/bin/chromedriver

RUN wget -q -O chrome.deb https://dl.google.com/linux/chrome/deb/pool/main/g/google-chrome-stable/google-chrome-stable_${CHROME_VERSION}-${DEBVERSION}_amd64.deb \
  && dpkg -i chrome.deb \
  && rm chrome.deb

USER 1200
