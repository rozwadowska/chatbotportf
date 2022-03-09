# chatbotportf

print ("Hej. To krotki program z rzeczami, ktorych sie nauczylam.")
imie = input("Na poczatek - poznajmy sie. Jak masz na imie?: ")
if (imie[-1] == 'a'):
    print("Dzieki", imie.capitalize(), "ze sie przedstawilas :)")
else:
    print ("Dzieki", imie.capitalize(), ",ze sie przedstawiles :)")
wiek = int(input ("A teraz powiedz mi, ile masz lat? ---> "))
zab = input("Masz ochote na prosta zabawe z obliczaniem wieku? tak/nie: ")
if (zab == 'tak'):
        liczba = int(input ("Ok. No to zabawa w dodawanie. Jaka liczbe chcesz dodac?: "))
        if (zab == 'tak'):
                print ("Najs.", wiek + liczba, "to jest wynik po dodaniu Twojego wieku.")
                wybor = input("Ok, to lecimy dalej. Pobawimy sie w kalkulator. Wybierz operacje: + to dodawanie, - to odejmowanie\
* to mnożenie, / to dzielenie. ---> ")
elif (zab == 'nie'):
    wybor = input("Ok, to lecimy dalej. Pobawimy sie w kalkulator. Wybierz operacje: + to dodawanie, - to odejmowanie\
* to mnożenie, / to dzielenie. ---> ")

a = int(input ("Pierwsza liczba: "))
b = int(input ("Druga liczba: "))

if (wybor == '+'):
    print ("Twoj wynik to:", a + b)
elif (wybor == '-'):
    print ("Twoj wynik to:", a - b)
elif (wybor == '/'):
    if (b == 0):
        print ("Tak to się nie bawimy ;)")
    else:
        print (a / b)
elif (wybor == '*'):
    print ("Twoj wynik to:", a * b)
print ("Ostatnie zadanie. Zwrocimy cene zawierajaca podatek VAT.")

VAT = 23
obliczonyVAT = (1 + VAT / 100)

cenaNetto = int(input ("Dla wybranej przez Ciebie ceny wolnej od podatku:  "))
cenaBrutto = cenaNetto * obliczonyVAT
print ("Cena brutto wynosi: ", cenaBrutto, "I to by było na dzisiaj tyle ;) Dzięki!")
