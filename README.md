01 void main()
02 {
03     system_init();
04 
05     SPI_Lcd_Out(1, 6, "mikroE");
06     SPI_Lcd_Out(2, 2, "LCD mini click");
07 
08     set_bcklight(0xFF);
09     set_contrast(0xDF);
10 
11     Delay_ms(5000);
12 
13     while (1)
14     {
15         set_bcklight(value);
16         set_contrast(value);
17 
18         value++;
19         delay_ms(40);
20     }
21 }
