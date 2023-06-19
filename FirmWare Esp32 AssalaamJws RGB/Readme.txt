ESP32 ASSALAAM-JWS FIRMWARE

1. Firmware terdiri 2 file : file utama dan file partision ( esp32 4MB dan 8MB sesuaikan esp32 
    yg digunakan ) file utama addrs = 0x10000 , file patision addrs= 0x8000.

2. firmware suport 1-6 panel P5 dan 1-10 panel p10 ( tergantung versi lisensi yg masukan )
    Untuk P10 ( 1Hub ada 5 pilihan SCAN, dan 2hub hayan ada 3 pilihan SCAN, scan No.urut )

3. config PCB :    ( pcb umum dipasaran ) / PCB Kalifah
    	PinOut HUB-75 : 		PinOut RTC :
	- R1 -> GPIO19		- RTC suport DS3231 & seiko epson ( RX-25... )
	- R2 -> GPIO5		   auto boot RTC
	- B1 -> GPIO18		- SDA -> GPIO 21
	- B2 -> GPIO17		- SDA -> GPIO 22
	- G1 -> GPIO13
	- G2 -> GPIO12
	- A    -> GPIO16
	- B   -> GPIO14
	- C   -> GPIO4
	- D   -> GPIO27
	- E   -> GPIO25
	- CLK -> GPIO2
	- OE -> GPIO15
	- LAT HUB-A -> GPIO26
	- LAT HUB-B -> GPIO23
	- Buzzer -> GPIO32

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