[john_passerelle2_privee.py](https://github.com/user-attachments/files/30625659/john_passerelle2_privee.py)
## Description
Mon projet d'IA locale connectée à un serveur de déploiement continu.

## Architecture
- **GitHub :** Sauvegarde et codage sécurisé.
- **Serveur Cloud (Unnug) :** Synchro automatique en arrière-plan
- [Uploading john_ai_paimport os


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
pip install litellm hugginface
import os
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
[sisi.py](https://github.com/user-attachments/files/30625666/sisi.py)
[texte.py](https://github.com/user-attachments/files/30625667/texte.py)
[profil_voix_patron.wav](https://github.com/user-attachments/files/30625687/profil_voix_patron.wav)
[passerelle_v9.py](https://github.com/user-attachments/files/30625686/passerelle_v9.py)
[nngrok.py](https://github.com/user-attachments/files/30625685/nngrok.py)
[memoire_vive.txt](https://github.com/user-attachments/files/30625684/memoire_vive.txt)
[memoire_lia.json](https://github.com/user-attachments/files/30625683/memoire_lia.json)
[memoire.txt](https://github.com/user-attachments/files/30625682/memoire.txt)
[maas.py](https://github.com/user-attachments/files/30625681/maas.py)
[johnnnnnnnnnn.txt](https://github.com/user-attachments/files/30625680/johnnnnnnnnnn.txt)
[johnnnnnnnnnn.py](https://github.com/user-attachments/files/30625679/johnnnnnnnnnn.py)
[john_v8.py](https://github.com/user-attachments/files/30625678/john_v8.py)
[john_v7.py](https://github.com/user-attachments/files/30625677/john_v7.py)
[john_v6.py](https://github.com/user-attachments/files/30625676/john_v6.py)
[john_v5.py](https://github.com/user-attachments/files/30625675/john_v5.py)
[john_v4.py](https://github.com/user-attachments/files/30625674/john_v4.py)
[john_passerelle2_privee.py](https://github.com/user-attachments/files/30625673/john_passerelle2_privee.py)
[john_passerelle_privee.py](https://github.com/user-attachments/files/30625672/john_passerelle_privee.py)
[john_final.py](https://github.com/user-attachments/files/30625671/john_final.py)
[john_ai_v9_future_ready.py](https://github.com/user-attachments/files/30625670/john_ai_v9_future_ready.py)
[john_ai.starting.txt](https://github.com/user-attachments/files/30625669/john_ai.starting.txt)
<img width="640" height="480" alt="visage_patron" src="https://github.com/user-attachments/assets/170c2433-9b09-4072-87cf-7fc20ffedfb0" />
[trans.py](https://github.com/user-attachments/files/30625668/trans.py)

if __name__ == '__main__':
  [john_v6.py](https://github.com/user-attachments/files/30625663/john_v6.py)
  app.run(host='0.0.0.0', port=5000, debug=False)
