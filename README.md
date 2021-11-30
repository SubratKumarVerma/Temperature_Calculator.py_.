# Temperature_Calculator.py_.

#Choossing Temperature Scale
temp=input("Choose Temperature: \nCelsius = °C\nFerenhiat = °F\nKelvin = K"'\n')

degree=float(input("Enter the Degree number: "))
if temp=='°C':
	temp2=input("\vChoose Temperature to convert: \nFerenhiat = °F\nKelvin = K"'\n')

#Convert Celsius Code
	if temp2=='°F':
		f=(degree*1.8)+32
		f1="{:.2f}".format(f)
		print('\v',degree,"degree Celsius is equals" , f1, "degree Ferenhait")
	else:
		k=degree+273.15
		k1="{:.2f}".format(k)
		print('\v',degree,"degree Celsius is equals" , k1, "degree Kelvin")

# convert Ferenhait code
elif temp=='°F':
	temp3=input("\vChoose Temperature to convert: \nCelsius = °C\nKelvin = K"'\n')
	if temp3=='°C':
		c=(degree-32) * 5/9
		c1="{:.2f}".format(c)
		print('\v',degree,"degree Ferenheit is equals" , c1, "degree Celsius")
	else:
		k=(degree-32) * 5/9 + 273.15
		k1="{:.2f}".format(k)
		print('\v',degree,"degree Ferenheit is equals" , k1, "degree Kelvin")

# convert Kelvin code
elif temp=='K':
	temp4=input("\vChoose Temperature to convert: \nCelsius = °C\nFerenheit = °F"'\n')
	if temp4=='°C':
		c=(degree-273.15)
		c1="{:.2f}".format(c)
		print('\v',degree,"degree Kelvin is equals" , c1, "degree Celsius")
	else:
		f=(degree - 273.15) * 9/5 + 32
		f1="{:.2f}".format(f)
		print('\v',degree,"degree Kelvin is equals" , f1, "degree Ferenheit")
