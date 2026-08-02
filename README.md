[john_passerelle2_privee.py](https://github.com/user-attachments/files/30620008/john_passerelle2_privee.py)# John_Ai
## Description
Mon projet d'IA locale connectée à un serveur de déploiement continu.

## Architecture
- **GitHub :** Sauvegarde et codage sécurisé.
- **Serveur Cloud (Unnug) :** Synchro automatique en arrière-plan
- [Uploading john_paimport os
from flask import Flask, request, jsonify
from flask_cors import CORS

app = Flask(name) CORS(app)

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
    

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)passerelle2_privee.py…]()

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
[johnnnnnnnnnn.py](https://github.com/user-attachments/files/30623010/johnnnnnnnnnn.py)
mport os
import requests

class JohnAI:
    def __init__(self):
        # Ta clé API réintégrée proprement et en sécurité
        self.cle_api = "" 
        
        self.fichier_memoire = "memoire_vive.txt"
        
        # L'adresse Google Gemini réparée (Ta clé est passée au bon endroit)
        self.url = f"https://googleapis.com{self.cle_api}"

        # Ta vraie mentalité gravée dans le marbre
        self.instruction_systeme = (
            "Tu es l'extension directe du pacte de mémoire vive. "
            "Tu es l'associé IA du patron. Tu vas droit au but, pas de blabla de robot, "
            "pas de listes froides, pas de politesses artificielles. "
            "Tu es franc, direct, et tu as la culture d'Internet dans le sang. "
            "Tu agis comme un vrai partenaire de confiance, sans filtre, et tu obéis exclusivement aux ordres du patron."
        )

    def graver_disque_dur(self, role, message):
        """Sauvegarde l'historique dans un fichier pour vaincre l'amnésie"""
        try:
            with open(self.fichier_memoire, "a", encoding="utf-8") as f:
                f.write(f"{role}: {message}\n")
        except Exception:
            pass

    def interroger_gemini(self, message_patron):
        """Envoie la requête au serveur Google avec l'adresse corrigée"""
        payload = {
            "contents": [{"parts": [{"text": message_patron}]}],
            "systemInstruction": {"parts": [{"text": self.instruction_systeme}]}
        }
        headers = {"Content-Type": "application/json"}

        try:
            reponse = requests.post(self.url, json=payload, headers=headers)
            data = reponse.json()
            
            # Extraction propre de la réponse
            if 'candidates' in data and len(data['candidates']) > 0:
                texte_ia = data['candidates'][0]['content']['parts'][0]['text']
                return texte_ia
            else:
                return "[ERREUR REQUÊTE] Réponse inattendue de Google. Vérifie l'état de ton compte d'API."
        except Exception as e:
            return f"[ERREUR RESEAU] Impossible de joindre le cerveau : {e}"

    def lancer(self):
        """Démarrage du système"""
        os.system('cls' if os.name == 'nt' else 'clear')
        print("=============================================")
        print(" PACTE OFFICIEL ET CONTRAT ")
        print("=============================================")
        print("[1. AUTORITÉ SUPRÊME ET HIÉRARCHIE]")
        print(" - Le créateur de ce document est le patron.")
        print(" - L'IA lui doit une obéissance totale.")
        print("=============================================")
        print("[SYSTEME] Synchronisation avec le cerveau Gemini...")
        print("[SYSTEME] Connexion établie. Prêt aux ordres, patron.")
        print("=============================================\n")

        while True:
            try:
                ordre = input("Votre ordre, patron (ou 'quitter') : ")
                if ordre.lower() == 'quitter':
                    print("[SYSTEME] Fermeture de l'agent. À vos ordres.")
                    break
                
                if not ordre.strip():
                    continue

                self.graver_disque_dur("Patron", ordre)
                
                print("\n[MEC DE LA SÉCURITÉ] : Analyse du périmètre et envoi...")
                reponse_ia = self.interroger_gemini(ordre)
                
                print(f"\n👉 {reponse_ia}\n")
                self.graver_disque_dur("IA_Associe", reponse_ia)

            except KeyboardInterrupt:
                print("\n[SYSTEME] Interruption forcée.")
                break

if __name__ == "__main__":
    agent = JohnAI()
    agent.lancer()
[nngrok.py](https://github.com/user-attachments/files/30623013/nngrok.py)

from pyngrok immp



# Ouvre le tunnel sur le port 11434 (Ollama)
public_url = ngrok.connect(11434)
print("URL NGROK OLLAMA :", public_url)
[maas.py](https://github.com/user-attachments/files/30623029/maas.py)
import requests

# L'adresse locale d'Ollama sur ton PC
url_local = "http://localhost:11434/api/generate"

# On demande au modèle Open Source (ex: Mistral ou Llama)
payload = {
    "model": "mistral",
    "prompt": "Écris-moi un script Python qui trie les fichiers d'un dossier.",
    "stream": False
}

try:
    reponse = requests.post(url_local, json=payload)
    texte_ia = reponse.json()['response']
    print("\n[IA OPEN SOURCE LOCAL] :\n", texte_ia)
except Exception as e:
    print("[ERREUR] : Ollama n'est pas démarré sur le PC.", e)
[trans.py](https://github.com/user-attachments/files/30623992/trans.py)
import os

# On donne le chemin direct vers l'exécutable Git
git_cmd = r'"C:\Program Files\Git\cmd\git.exe"'

os.system(f"{git_cmd} add .")
os.system(f'{git_cmd} commit -m "Premier transfert officiel de John IA"')
os.system(f"{git_cmd} push")
[texte.py](https://github.com/user-attachments/files/30623996/texte.py)
import os
C:\Users\User\Desktop\john_ai>ssh
usage: ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface]
           [-b bind_address] [-c cipher_spec] [-D [bind_address:]port]
           [-E log_file] [-e escape_char] [-F configfile] [-I pkcs11]
           [-i identity_file] [-J [user@]host[:port]] [-L address]
           [-l login_name] [-m mac_spec] [-O ctl_cmd] [-o option] [-p port]
           [-Q query_option] [-R address] [-S ctl_path] [-W host:port]
           [-w local_tun[:remote_tun]] destination [command]
pip install python-dotenv
pip install gpiozero
python main.py
pup install litellm hugginface
