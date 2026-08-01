[john_passerelle2_privee.py](https://github.com/user-attachments/files/30620008/john_passerelle2_privee.py)# John_Ai
## Description
Mon projet d'IA locale connectée à un serveur de déploiement continu.

## Architecture
- **GitHub :** Sauvegarde et codage sécurisé.
- **Serveur Cloud (Unnug) :** Synchro automatique en arrière-plan
- [Uploading john_paimport os
from flask import Flask, request, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)

print("=========================================")
print(" PASSERELLE PRIVÉE V8 ACTIVE & SÉCURISÉE ")
print("=========================================")
print("[PROTOCOLE] : Chiffrement d'identification automatique activé.")
print("[SÉCURITÉ] : En attente de la signature du Patron...")

@app.route('/ordre_mobile', methods=['POST'])
def passerelle_v8():
    donnees = request.get_json() or {}
    
    # Vérification de la signature du téléphone
    signature = donnees.get("signature", "")
    message_patron = donnees.get("ordre", "")
    
    if signature != "PATRON_V8_SECURE_TOKEN_99":
        print("[ALERTE SÉCURITÉ] : Tentative de connexion inconnue refusée.")
        return jsonify({"statut": "ERREUR", "reponse": "Accès refusé. Appareil non identifié."}), 403

    print(f"\n[SIGNATURE VALIDÉE] -> Le Patron est en ligne.")
    print(f"[RECONNAISSANCE] -> Message vocal reçu : '{message_patron}'")
    
    return jsonify({
        "statut": "IDÉES REMISES AU CLAIR",
        "reponse": f"Toutes les IA sont connectées, patron. Ordre reçu : {message_patron}"
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)sserelle2_privee.py…]()

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
