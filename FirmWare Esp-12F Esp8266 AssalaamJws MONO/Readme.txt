ESP8266 ASSALAAM-JWS FIRMWARE

1. Firmware terdiri 1 file .BIN 

2. *firmware P10 1HUB12 suport 1-10 panel ( tergantung versi lisensi yg masukan )
    *firmware P10 2HUB12 suport 1-10 panel ( tergantung versi lisensi yg masukan )

3. config PCB :   ESP8286 / Esp-12F
    	PinOut HUB-12 : 		PinOut RTC :
	- OE -> GPIO15		- RTC suport DS3231 & seiko epson ( RX-25... )
	- R1 -> GPIO13 ->HUB1	   auto boot RTC
	- R2 -> GPIO3  ->HUB2	- SDA -> GPIO 4
	- LAT -> GPIO0		- SDA -> GPIO 5
	- CLK -> GPIO14
	- Buzzer -> GPIO2

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