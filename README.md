wizard = "wizard"
elf = "elf"
human = "human"
dragon = "dragon"

wizard_hp = 70
elf_hp = 100
human_hp = 150

wizard_damage = 150
elf_damage = 100
human_damage = 20

dragon_hp = 300
dragon_damage = 50


while True:
   print("1)human")
   print("2)wizard")
   print("3)elf")
   
   character = input("choose your character: ")
   if character == "1":
       print("you have chosen human!")
       my_hp = human_hp 
       print(f"health: {my_hp}")
       my_damage = human_damage
       print(f"damage: {my_damage}")
       break
   if character == "2":
       print("you have selected wizard!")
       my_hp = wizard_hp 
       print(f"health: {my_hp}")
       my_damage = wizard_damage
       print(f"damage: {my_damage}")
       break
   if character == "3":
       print("you have selected elf!")
       my_hp = elf_hp 
       print(f"health: {my_hp}")
       my_damage = elf_damage
       print(f"damage: {my_damage}")
       break

while True:
    if character == "1":
       print("The human", "damaged the Dragon!")
       print("The", dragon, "damaged the human!")
       dragon_hp = dragon_hp - my_damage
       print(f"dragon health: {dragon_hp}")
       my_hp = my_hp - dragon_damage
       print(f"human health: {my_hp}")
    if character == "2":
      print("The wizard", "damaged the Dragon!")
      print("The", dragon, "damaged the wizard!")
      dragon_hp = dragon_hp - my_damage
      print(f"dragon health: {dragon_hp}")
      my_hp = my_hp - dragon_damage
      print(f"wizard health: {my_hp}")
    if character == "3":
      print("The", elf, "damaged the Dragon!")
      print("The", dragon, "damaged the elf!")
      dragon_hp = dragon_hp - my_damage
      print(f"dragon health: {dragon_hp}")
      my_hp = my_hp - dragon_damage
      print(f"elf health: {my_hp}")
    
    
    if my_hp <= 0:
       print("you lose")
       break
    if dragon_hp <= 0:
       print("you win")
       break
    
