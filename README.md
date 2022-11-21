# Kekw
class Discord:
##atributos##
##Fin de atributos##

##Inicio del constructor## ##Clase ##
    def __init__(self,id,nickname,avatar,status,creaat,mail,premium=False):
        self.id = id
        self.nickname = nickname 
        self.avatar = avatar    
        self.status = status    
        self.creaat = creaat
        self.mail =mail
        self.premium = premium
        
    def print(self):
        print("el id es:"+str(self.id))
        print("el avatar es"+str(self.avatar))
        print("La fecha de creacion es:"+str(self.creaat))
        print("el Seudonimo es:"+str(self.nickname))
        print("el Estado actual de su cuenta es:"+str(self.premium))
    





from discord import Discord
def main():
    ids = int(input("Ingrese la id"))
    avatar = str(input("Ingrese su foto .png"))
    creaat = str(input("Ingrese su fecha de creSacion de la cuenta"))
    nickname = str(input("Ingrese su seudonimo"))
    premium = bool(input("Ingrese su estado online,Conectado,Ausente,Ocupado,Desconectado"))
    status = str(input("Ingrese si es premium onoxd"))

    user = Discord(ids,avatar,creaat,nickname,premium,status)
    user.print()
main()
