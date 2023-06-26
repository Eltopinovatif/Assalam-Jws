ESP32 ASSALAAM-JWS FIRMWARE

1. Firmware terdiri 2 file : file utama dan file partision ( esp32 4MB dan 8MB sesuaikan esp32 
    yg digunakan ) file utama addrs = 0x10000 , file patision addrs= 0x8000.

2. firmware suport 1-6 1HUB-2HUB panel P5 , dan 3HUB 3x3-4-5-6Panel P5 ( tergantung versi lisensi yg masukan )
    
3. config PCB :    ( pcb umum dipasaran ) / PCB Kalifah
    	PinOut HUB-75 : 		PinOut RTC :
	- R1 -> GPIO2		- RTC suport DS3231 & seiko epson ( RX-25... )
	- R2 -> GPIO16		   auto boot RTC
	- B1 -> GPIO4		- SDA -> GPIO 32
	- B2 -> GPIO17		- SCL -> GPIO 33
	- G1 -> GPIO15
	- G2 -> GPIO27
	- A    -> GPIO5
	- B   -> GPIO18
	- C   -> GPIO19
	- D   -> GPIO21
	//- E   -> GPIO25
	- CLK -> GPI022
	- OE -> GPIO25
	- LAT HUB-A -> GPIO26
	- LAT HUB-B -> GPIO13
 	- LAT HUB-C -> GPIO23
	- LAT HUB-D -> GPIO0
	- Buzzer -> GPIO12

4. Master Reset [ Hard RESET = pin RX dan GRN ] atau soft RESET [ app RESET paswd= "99999999" ]
	- jika data crash / kacau bisa direset dg Hard RESET atau soft RESET.
	- jika lupa Password WiFi hanya bisa dg Hard Reset.
	* Cara Hard RESET : Pin RX dan GRN di Jumper / disambung Lalu Power dinyalakan dan Bunyi
	   		    BEEP 2x, maka Reset Sukses. seting kembali ke seting Default / Factory

5. APP dan Manual Book :
	# https://play.google.com/store/apps/detailsid=io.kodular.herrysantoso2012.As_salaamJws
		* Soft Password = "9999"
		* WiFi Password Default = "12345678"
	# https://assalaamjws.blogspot.com/

6. Lisensi :
	- contac : 089401338686
7. link pembelian PCB : https://www.tokopedia.com/micro-ten/pcb-jws-rgb-esp32-4hub?extParam=whid%3D5949468
