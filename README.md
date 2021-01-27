while True:
    degree, conversion = input("enter the temprature you like to convert (for example 10 f or 29 C etc...)\n").split()
    conversiont1 = 0
    conversiont2 = 0
    r1 = 0
    r2 = 0
    if conversion == "0":
        break
    elif conversion.upper() == "C":
        r1 = (9 * int(degree)) / 5 + 32
        r2 = (int(degree)+273.15)
        conversiont1 = "Fahrenheit"
        conversiont2 = 'Kelvin'
        print("The temprature in", conversiont1, "is", r1, "degrees and", conversiont2, "is", r2, "Degrees")

    elif conversion.upper() == "F":
        r1 = (int(degree)-32)*5/9
        r2 = (int(degree)-32)*5/9+273.15
        conversiont1 = "Celsius"
        conversiont2 = 'Kelvin'
        print("The temprature in", conversiont1, "is", r1, "degrees and", conversiont2, "is", r2, "Degrees")

    elif conversion.upper() == "K":
        r1 = (int(degree)-273.15)
        r2 = (int(degree)*9/5-459.67)
        conversiont1 = "Celsius"
        conversiont2 = "Fahrenheit"
        print("The temprature in", conversiont1, "is", r1, "degrees and", conversiont2, "is", r2, "Degrees")

    else:
        print("invalid input")
