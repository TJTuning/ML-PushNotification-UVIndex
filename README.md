# ML-PushNotification-UVIndex

TITLE:
Auto-Push Notification Service for Vitamin D Deficiency Based on UV Index (And an Attempt To Create Predictive Models Using Data From A Weather API)

1) Set-up: Raspberry Pi 4B connected to an ethernet switch - configured via a Python script to get the latest weather data in JSON from a web API and store in a MySQL database
2) After each run, calculate average of predicted UV index throughout 7 days and if low ( < 3 ) send push notification to phone
3) Sequentially a linear regression model will run based on the training and testing splits of the historical dataset

Script will run on a 5-min interval using a cron job (time-based job scheduler)

