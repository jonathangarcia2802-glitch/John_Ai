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
