def calculator():
    print("Jednoduchá Python kalkulačka")
    print("Dostupné operace: +, -, *, /")
    print("Pro ukončení zadej 'q'.\n")

    while True:
        vstup = input("Zadej příklad (např. 5 + 3) nebo 'q' pro konec: ")
        if vstup.lower() == 'q':
            print("Kalkulačka se ukončuje.")
            break

        try:
            casti = vstup.split()
            if len(casti) != 3:
                raise ValueError("Neplatný formát. Použij tvar: číslo operátor číslo (např. 5 + 3)")

            num1 = float(casti[0])
            operator = casti[1]
            num2 = float(casti[2])

            if operator == '+':
                vysledek = num1 + num2
            elif operator == '-':
                vysledek = num1 - num2
            elif operator == '*':
                vysledek = num1 * num2
            elif operator == '/':
                if num2 == 0:
                    print("Chyba: Nelze dělit nulou!")
                    continue
                vysledek = num1 / num2
            else:
                print(f"Chyba: Neznámý operátor '{operator}'. Použij +, -, *, /")
                continue

            print(f"Výsledek: {vysledek}\n")

        except ValueError as e:
            print(f"Chyba: {e}\n")

if __name__ == "__main__":
    calculator()
