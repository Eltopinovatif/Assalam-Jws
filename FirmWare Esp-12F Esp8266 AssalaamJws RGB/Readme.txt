ESP8266 ASSALAAM-JWS FIRMWARE

1. Firmware terdiri 3 file .BIN 

2. *firmware P5-P10 1HUB75 suport 1-6 panel P5 dan 1-10 panel p10 ( tergantung versi lisensi yg masukan )
    *firmware P5-2HUB75 suport 1-5 panel P5  ( tergantung versi lisensi yg masukan )
    *firmware P10-2HUB75 suport 1-10 panel p10 ( tergantung versi lisensi yg masukan )

3. config PCB :   ESP8286 / Esp-12F
    	PinOut HUB-75 : 		PinOut RTC :
	- R1 -> GPIO15		- RTC suport DS3231 & seiko epson ( RX-25... )
	- R2 -> GPIO3		   auto boot RTC
	- B1 -> GPIO5		- SDA -> GPIO 2
	- B2 -> GPIO13		- SDA -> GPIO 0
	- G1 -> GPIO4
	- G2 -> GPIO13
	- A    -> 74HC595 pin4
	- B   -> 74HC595 pin5
	- C   -> 74HC595 pin6
	- D   -> 74HC595 pin7
	- CLK -> GPIO2
	- OE -> GPIO15
	- LAT HUB-A -> GPIO10
	- LAT HUB-B -> GPIO1
	- Buzzer -> 74HC595 pin15

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
7. link pembelian PCB : https://www.tokopedia.com/archive-bimotech-1651126636/pcb-jws-rgb-esp12-pcb-jam-masjid-rgb
