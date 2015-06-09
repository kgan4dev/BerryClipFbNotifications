# BerryClipFbNotifications
It lets a berry Clip IoT Applications to give notifications of Facebook Profile when push button get pressed.

# Install Dependencies
Install python-pip package if not installed already

$ sudo apt-get install python-pip

then, install dependencies for 'BerryClipFbNotifications'.

$ pip install -r requirements.txt

# Running 'BerryClipFbNotifications' application.

$ sudo python app.py

# Use tunneling to expose this local app on public
Just for temporary purpose, We use 'ngrok' in this case.

Download ngrok binary from their site. (On Raspberry Pi only)

$ wget https://dl.ngrok.com/ngrok_2.0.19_linux_arm.zip

$ unzip ngrok_2.0.19_linux_arm.zip

$ ./ngrok http 3396

then, you can see a sub-domain URL on ngrok for your local application

Example:  https://xxxxxxx.ngrok.io

Copy and paste that on web browser. You can see Berry Clip device controls with image.

# How to register this app on FaceBook.?

1. Goto https://developers.facebook.com and if not logged in, login with your user id and password & Register yourself as facebook developer.

2. Goto 'My Apps' and Create a new app on your facebook. You will get pop-up to select particular application. From there, Click on 'Facebook Canvas' type.

3. Then, Enter your application name. Something like, 'Vedams IoT Device'. and Create AppID for that while choosing category as any of your choice. 

4. After that, You will see 'Where is your app hosted?'. In this case, 
	Secure Host URL
		Enter the sub-domain URL of ngrok
		Ex: https://xxxxxxx.ngrok.io/

Click Submit and then Next. Then, Open your app. 

Finally, You could see a notification 'Vedams Pi BerryClip app is loaded.'
