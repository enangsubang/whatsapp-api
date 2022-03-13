Whatsapp API Tutorial - Please check me intervally. Scripts would be updated anytime - 

=== NOTE : OPEN THIS FILE IN RAW/TEXT/CODE MODE FOR BEST DETAIL VIEWS ===

A. WINDOWS
--------------------------------------------------------------------------
1. Download Window Installer Node JS Ver >= 12 + NPM : https://nodejs.org/en/download/
2. Make sure version nodejs >= V.12+ : node -v
3. Download and install git on windows https://git-scm.com/downloads
4. Open Command Prompt (as an administrator)
5. git clone https://github.com/enangsubang/whatsapp-api.git
6. cd whatsapp-api
7. npm install puppeteer
8. npm i whatsapp-web.js
9. npm i express-fileupload
10. npm install
11. npm run start
12. Access URL : http://localhost:8000 or Access URL : http://IP_SERVER:8000
13. Make sure the qr code appears
14. Open your device (Smartphone). Open Whatsapp App, Enter Configuration, Scan QR.
15. If everythings is OK, your WA-API is ready to go... 

==========================================================================

B. Linux Ubuntu
--------------------------------------------------------------------------
1. Install Node JS 12	
	sudo apt-get install software-properties-common
	curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
	sudo apt-get install nodejs
	node -v 
	sudo apt update
2. apt install npm -y
3. npm install -g npm@latest
4. apt-get install git -y
5. git clone https://github.com/enangsubang/whatsapp-api.git
6. cd whatsapp-api/
7. sudo apt install -y gconf-service libasound2 libatk1.0-0 libatk-bridge2.0-0 libc6 libcairo2 libcups2 libdbus-1-3 libexpat1 libfontconfig1 libgcc1 libgconf-2-4 libgdk-pixbuf2.0-0 libglib2.0-0 libgtk-3-0 libnspr4 libpango-1.0-0 libpangocairo-1.0-0 libstdc++6 libx11-6 libx11-xcb1 libxcb1 libxcomposite1 libxcursor1 libxdamage1 libxext6 libxfixes3 libxi6 libxrandr2 libxrender1 libxss1 libxtst6 ca-certificates fonts-liberation libappindicator1 libnss3 lsb-release xdg-utils wget
8. 	sudo apt-get update
	sudo apt-get install -y libgbm-dev
9. npm install puppeteer
10. npm i whatsapp-web.js
11. npm i express-fileupload
12. npm install
13. npm run start
14. Access URL : http://IP_SERVER:8000
15. Make sure the qr code appears
16. Open your device (Smartphone). Open Whatsapp App, Enter Configuration, Scan QR.
17. If everything is OK, your WA-API is ready to go... 

API COMMAND TEST 
=== NOTE : OPEN THIS FILE IN RAW/TEXT/CODE MODE FOR BEST DETAIL VIEWS ===
-------------------------------------------------------------------------------------------
1. Test via App : Postman Canary
2. Send Text Message
   URL Access : http://IP_SERVER:8000/send-message
    Method : Post
    Body : form-data
     KEY    : VALUE
    -----------------------
    number  : 62823xxxxxxx
    message : Test Message 1234
   
   Klik Send

3. Send File 
    URL Access :  http://IP_SERVER:8000/send-media
    Method : Post
    Body : form-data
     KEY    : VALUE
    -----------------------
    number  : 62823xxxxxxx
    caption : Test Media Sending
    file    : http://3.bp.blogspot.com/-Uz_fFLM8uAY/UWFq1dST2lI/AAAAAAAAANM/BUmc9xk84b4/s1600/Esapicture--0096.jpg
   
   Klik Send
   
4. Clear Message
    URL Access : http://IP_SERVER:8000/clear-message
    Method : Post
    KEY    : VALUE
    -----------------------
    number : 62823xxxxxxx
    
    Klik Send  
    
5. Reset Session/Device/QR
    URL Access : http://IP_SERVER:8000/reset
    Method : Post
    Klik Send  
      
    
Use c-Url In PHP :

<?php
  	$url = 'http://IP_SERVER:8000/send-message';
	$data = array(
			'number' => '62823xxxxxxx',
			'message'  => 'this is sample message',
		);
   	$data_string = json_encode($data);
 	$ch = curl_init($url);
	curl_setopt($ch, CURLOPT_CUSTOMREQUEST, "POST");
	curl_setopt($ch, CURLOPT_POSTFIELDS, $data_string);
	curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
	curl_setopt($ch, CURLOPT_VERBOSE, 0);
	curl_setopt($ch, CURLOPT_CONNECTTIMEOUT, 0);
	curl_setopt($ch, CURLOPT_TIMEOUT, 360);
	curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, 0);
	curl_setopt($ch, CURLOPT_SSL_VERIFYHOST, 0);
	curl_setopt(
		$ch,
		CURLOPT_HTTPHEADER,
		array(
			'Content-Type: application/json',
			'Content-Length: ' . strlen($data_string)
		)
	);
	echo $res = curl_exec($ch);
	curl_close($ch);
?>


 ========== UNINSTALL NODEJS ===
sudo apt-get remove nodejs
sudo apt-get purge nodejs
sudo apt-get autoremove



DONATING SUPPORT
-------------------------------------------------------------------------------------------
Found this project helpful and want to give a support by donating?

You can donate directly to my bank account below.

Bank name: Bank BCA [ code: 014 ]
Account number: 055 055 8424
Receiver name: Enang Sumarna

OR

GOPAY : 70001082318765334

Feel free to contact me by Whatsapp: 6282318765334. Maybe for the transfer confirmation, so I know about your support.

Thanks in advance.
