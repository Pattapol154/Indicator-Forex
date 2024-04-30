# Indicator-Forex

rsi idea 
1. เล่นเเบบเดิม
   rsi >= 70 open sell
   rsi <= 30 open buy
   *ข้อเสีย : มันมีความเสี่ยงสูงมากที่จะเกิด overbought , oversold
2. เล่นแบบใหม่
   rsi = 50 เป็นฐาน เเนวรับ,เเนวต้าน
   if rsi > 50 open buy follow ตามกราฟ
               close buy เมื่อเกิด overbought , tp profit
   if rsi < 50 open sell follow ตามกราฟ
               close sell เมื่อเกิด oversold , tp profit

   if in case open buy ผิดทาง
               check current position rsi < 50 close buy , open sell
   if in case open sell ผิดทาง
               check current position rsi > 50 close sell , open buy
