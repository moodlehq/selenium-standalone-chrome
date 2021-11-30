FROM selenium/standalone-chrome:96.0

USER root
COPY chromedriver /opt/selenium/chromedriver-96.0.4664.45-moodlehq
RUN rm /usr/bin/chromedriver && \
    ln -s /opt/selenium/chromedriver-96.0.4664.45-moodlehq /usr/bin/chromedriver

USER 1200
