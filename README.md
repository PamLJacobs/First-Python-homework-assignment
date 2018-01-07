weight_today = float(input ("enter today's weight:"))
print
weight_yesterday = float(input ("enter yesterday's weight:"))
print
fat_per_today = float(input ("enter today's fat pct:"))
print
fat_per_yesterday = float(input ("enter yesterday's fat pct:"))
print
if weight_today < weight_yesterday:
  print ("pounds lost:", round(weight_yesterday - weight_today,1))
elif weight_today > weight_yesterday:
  print ("pounds gained:", round(weight_today - weight_yesterday,1))
else:
  print ("same weight as yesterday")
fat_weight_today = weight_today*.01*fat_per_today
fat_weight_yesterday = weight_yesterday*.01*fat_per_yesterday
fat_loss = fat_weight_today - fat_weight_yesterday
if fat_weight_today < fat_weight_yesterday:
   print ("fat pounds lost:", round(fat_loss,1)," Great Job!")
else: 
   print ("oink")
