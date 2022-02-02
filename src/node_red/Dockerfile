FROM nodered/node-red:latest
USER root
RUN npm i node-red-dashboard
RUN npm install node-red-contrib-ui-state-trail
RUN npm install node-red-contrib-ui-reef
RUN npm install node-red-contrib-ui-led
RUN npm install node-red-contrib-light-scheduler
USER node-red
