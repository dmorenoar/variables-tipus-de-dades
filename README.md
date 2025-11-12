# 👨‍🎓 Tipus de dades

Definim una variable posant-li nom i assignant un valor amb =
en python no hem d'especificar el tipus de dada.

## ♦️ int (enters) - Són nombres sense part decimal.
```python
number = 10
numberTwo = -3
numberThree = 0
```

## ♦️ str (string) - Són cadenes de text, entre cometes simples o dobles.
```python
name = 'Dani'
pokemon = "Pikachu"
letter = 'A'
```

## ♦️ bool (booleà) - Només poden tenir dos valors: True o False.
```python
isAdmin = True
isShiny = False
```

## ♦️ float (decimals) - Són nombres amb part decimal.
```python
price = 10.99
pi = 3.1416
temperature = -2.5
```

## ♦️ Mostrar dades per pantalla

### Print s'utilitza per mostrar dades per pantalla

**Mostra un text per pantalla:**
```python
print('Hola')
print("Welcome!")
```

**Mostra un text i variables amb concatenació +**
Funciona només amb cadenes (str), per tant cal convertir números a text amb str().
```python
print('El pokemon ' + pokemon + ' és de tipus elèctric')
print('La temperatura és de ' + str(temperature))
```

**Mostra un text i variables amb ,**
Python afegeix un espai automàtic entre cada element.
```python
print("Nom:", name, " - isAdmin:", isAdmin)
```

**Mostra un text amb f-strings (la manera més moderna i recomanada)**  
Només cal posar una f davant les cometes i escriure les variables entre { }.
```python
print(f"Nom: {name}")
print(f"El teu nom d'entrenador és {name} i el teu pokemon {pokemon}")
```

**També podem fer operacions directament al mostrar les variables:**
```python
print("El preu és " + str(price + 10))
print(f"El preu és {price + 10}")
```

## ♦️ Lectura de dades de l'usuari

### Llegir un text (cadena)
```python
print('Com et dius?')
name_user = input()
print(f'El teu nom és {name_user}')
```

### Llegir i mostrar al mateix temps
```python
name_pokemon = input('Introdueix el nom del pokemon:')
print('El teu nom és ' + name_pokemon)
```

### Llegir nombres enters
```python
print('Introdueix el teu any de naixement:')
year_birthday = int(input())
print('Has nascut el', year_birthday)

year = int(input("Quina edat tens?"))
print(f'Tens {year} anys. El pròxim any tindràs {year + 1} anys')
```

### Llegir diversos valors separats en una sola línia
```python
name_entrenador, lucky_number = input("Introdueix el teu nom d'entrenador i el teu num de la sort").split()
print(f"El teu nom d'entrenador és {name_entrenador} i el teu num de la sort el {lucky_number}")
```

### Llegir diversos nombres separats en una sola línia
```python
b, h = map(int, input('Introdueix la base i altura:').split())
print(f'Has escrit base: {b} i altura:{h}')
print(f"L'àrea del triangle és {(b*h)/2}")
```

## ♦️ Operacions amb nombres

**Important fer servir parèntesis per respectar l'ordre:**
```python
print(5 + 10)
print(3 * 7, (17 - 2) * 8)
```

**Dos asteriscs s'utilitzen per a l'exponenciació (N elevat a X):**
```python
print(2 ** 4)  # 2 elevat a 4
print(6 ** 2)  # 6 elevat a 2
```

**Una sola barra inclinada és una divisió:**
```python
print(37 / 3)
```

**Doble barra inclinada és una divisió entera**
Retorna només el quocient de la divisió (és a dir, sense residu):
```python
print(16 // 3)
```

**El signe de percentatge és un operador de mòdul**
Dóna el residu del valor de l'esquerra dividit pel valor de la dreta:
```python
print(10 % 2)
```

## ♦️ Operacions amb variables
```python
total_price = numberThree + number
print(f'El preu total és {total_price}')

pair_number = number % 2
print('El residu de ' + str(number) + ' dividit entre 2 és ' + str(pair_number))
