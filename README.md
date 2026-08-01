# John_Ai
## Description
Mon projet d'IA locale connectée à un serveur de déploiement continu.

## Architecture
- **GitHub :** Sauvegarde et codage sécurisé.
- **Serveur Cloud (Unnug) :** Synchro automatique en arrière-plan
import os
import requests

def verifier_connexion_systeme():
    print("--- VÉRIFICATION DES CONNEXIONS (PORT 5000) ---")
    
    # Vérification des variables d'environnement chargées
    ngrok_status = "Présente" if os.getenv("NGROK_AUTH_TOKEN") else "Manquante ou non détectée"
    api_status = "Présente" if os.getenv("API_KEY_PRIMARY") else "Manquante ou non détectée"
    
    print(f"-> Token Ngrok : {ngrok_status}")
    print(f"-> Clé API principale : {api_status}")
    print(f"-> Port cible : {os.getenv('TARGET_PORT', '5000 (par défaut)')}")
    
    print(f"-> Environnement : {os.getenv('HOSTING_ENVIRONMENT', 'Hugging Face')}")
    

    
    print("---------------------------------------------")

if __name__ == "__main__":
    verifier_connexion_systeme()
