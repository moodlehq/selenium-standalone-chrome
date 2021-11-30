FROM selenium/standalone-chrome:3.141.59-20210929

USER root
COPY chromedriver /opt/selenium/chromedriver-94.0.4604.61-moodlehq
RUN rm /usr/bin/chromedriver && \
    ln -s /opt/selenium/chromedriver-94.0.4604.61-moodlehq /usr/bin/chromedriver

USER 1200
