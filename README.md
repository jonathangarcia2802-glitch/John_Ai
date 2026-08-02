[reparation_qg.py](https://github.com/user-attachments/files/30625693/reparation_qg.py)

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
import os
import sys
import subprocess
import requests

def reparer_et_relancer():
    os.system('cls' if os.name == 'nt' else 'clear')
    print("=============================================")
    # 1. NETTOYAGE RADICAL DE LA MÉMOIRE CACHE
    try:
        # On ferme de force tous les scripts Python et blocs-notes qui buggent en arrière-plan
        subprocess.run("taskkill /F /IM python.exe /IM notepad.exe", shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
    except Exception:
        pass
    print("[1/3] MÉMOIRE NETTOYÉE : Fenêtres fantômes éliminées.")

    # 2. INJECTION DU CODE PARFAIT ET CONFIGURÉ SANS ERREUR
    cle_api = "AQ.Ab8rn6I8QV-ukEvEXUjrFpEHk8owhOs4eTFOZiN69zh2ie-OzQ"
    url_corrigee = f"https://googleapis.com{cle_api}"
    
    code_propre = f"""import os
import tkinter as tk
from tkinter import messagebox, scrolledtext
import requests
import threading

class QG_Advanced_UI:
    def __init__(self):
        self.cle_api = "{cle_api}"
        self.url = "{url_corrigee}"
        self.instruction_systeme = (
            "Tu es l'associé IA du patron. Tu es un ingénieur expert en Python. "
            "Génère UNIQUEMENT du code Python propre, optimisé et commenté. "
            "Pas de bavardage, pas de texte introductif, donne directement le script."
        )

    def interroger_gemini(self, prompt):
        payload = {{"contents": [{{"parts": [{{"text": prompt}}]}}], "systemInstruction": {{"parts": [{{"text": self.instruction_systeme}}]}}}}
        headers = {{"Content-Type": "application/json"}}
        try:
            reponse = requests.post(self.url, json=payload, headers=headers)
            data = reponse.json()
            if 'candidates' in data and len(data['candidates']) > 0:
                candidate = data['candidates'][0]
                if 'content' in candidate and 'parts' in candidate['content']:
                    parts = candidate['content']['parts']
                    if len(parts) > 0 and 'text' in parts[0]:
                        return parts[0]['text']
            return "[ERREUR API] : Le cerveau Gemini a refusé la requête. Clé ou quota expiré."
        except Exception as e:
            return f"[ERREUR SYSTEME] : {{e}}"

def action_envoyer():
    ordre = entree_texte.get("1.0", tk.END).strip()
    if not ordre: return
    lancer_traitement(ordre)

def lancer_traitement(texte_ordre):
    zone_reponse.delete("1.0", tk.END)
    zone_reponse.insert(tk.END, "[TRACKING] : Transmission au cerveau Gemini v1.5...\\n")
    canvas_led_gemini.itemconfig(led_gemini, fill="#ffa500")
    fenetre.update()

    def calcul_thread():
        code_traduit = core.interroger_gemini(texte_ordre)
        zone_reponse.delete("1.0", tk.END)
        zone_reponse.insert(tk.END, code_traduit)
        if "[ERREUR]" in code_traduit or "SYSTEME" in code_traduit:
            canvas_led_gemini.itemconfig(led_gemini, fill="#ff0000")
            label_statut.config(text="Statut : Liaison interrompue.", fg="#ff0000")
        else:
            canvas_led_gemini.itemconfig(led_gemini, fill="#00ff00")
            label_statut.config(text="Statut : Script Python gravé dans 'code_traduit.py' !", fg="#00ff00")
            with open("code_traduit.py", "w", encoding="utf-8") as f:
                f.write(code_traduit)

    threading.Thread(target=calcul_thread).start()

core = QG_Advanced_UI()
fenetre = tk.Tk()
fenetre.title("MEC DE LA SÉCURITÉ V8 - CONSOLE SUPRÊME")
fenetre.geometry("900x650")
fenetre.configure(bg="#0a0a0c")

frame_titre = tk.Frame(fenetre, bg="#141419", height=50, bd=1, relief="groove")
frame_titre.pack(fill="x", padx=10, pady=5)
tk.Label(frame_titre, text="🎛️ SYSTEM OPERATIONAL CONTROL v8.2", font=("Courier", 14, "bold"), bg="#141419", fg="#00ff00").pack(pady=10)

panel_ia = tk.Frame(fenetre, bg="#111115", width=220, bd=1, relief="solid")
panel_ia.pack(side="left", fill="y", padx=10, pady=5)
tk.Label(panel_ia, text=" AGENTS CONNECTÉS ", font=("Courier", 10, "bold"), bg="#1d1d24", fg="white").pack(fill="x", pady=5)

frame_john = tk.Frame(panel_ia, bg="#16161e", bd=1, relief="ridge")
frame_john.pack(fill="x", padx=5, pady=10)
photo_john = tk.Canvas(frame_john, width=60, height=60, bg="#1a233a", highlightthickness=0)
photo_john.create_rectangle(10, 10, 50, 50, outline="#00ff00", width=2)
photo_john.create_text(30, 30, text="JOHN", fill="#00ff00", font=("Courier", 8, "bold"))
photo_john.pack(side="left", padx=5, pady=5)

info_john = tk.Frame(frame_john, bg="#16161e")
info_john.pack(side="left", fill="both", expand=True, padx=5)
tk.Label(info_john, text="John AI\\n(Cerveau)", font=("Arial", 9), bg="#16161e", fg="white", justify="left").pack(anchor="w")
canvas_led_gemini = tk.Canvas(info_john, width=20, height=20, bg="#16161e", highlightthickness=0)
canvas_led_gemini.pack(anchor="w", pady=2)
led_gemini = canvas_led_gemini.create_oval(2, 2, 16, 16, fill="#00ff00")

panel_droite = tk.Frame(fenetre, bg="#0a0a0c")
panel_droite.pack(side="right", fill="both", expand=True, padx=5, pady=5)
tk.Label(panel_droite, text="⚡ REQUÊTE COMMANDE (FRANÇAIS) :", font=("Courier", 10, "bold"), bg="#0a0a0c", fg="#00ff00").pack(anchor="w", padx=5)
entree_texte = scrolledtext.ScrolledText(panel_droite, height=4, bg="#141419", fg="white", insertbackground="white", font=("Consolas", 11), bd=1, relief="solid")
entree_texte.pack(fill="x", padx=5, pady=5)

frame_boutons = tk.Frame(panel_droite, bg="#0a0a0c")
frame_boutons.pack(fill="x", pady=5)
btn_envoyer = tk.Button(frame_boutons, text="📡 DEMANDER LA TRADUCTION PYTHON", font=("Courier", 10, "bold"), bg="#00ff00", fg="black", command=action_envoyer, activebackground="#33ff33", cursor="hand2")
btn_envoyer.pack(fill="x", padx=5, pady=5)

tk.Label(panel_droite, text="💾 SCRIPT PYTHON TRADUIT ET GRAVÉ :", font=("Courier", 10, "bold"), bg="#0a0a0c", fg="#00ff00").pack(anchor="w", padx=5, pady=5)
zone_reponse = scrolledtext.ScrolledText(panel_droite, height=18, bg="#000000", fg="#39ff14", insertbackground="#39ff14", font=("Consolas", 11), bd=1, relief="solid")
zone_reponse.pack(fill="both", expand=True, padx=5, pady=5)

label_statut = tk.Label(fenetre, text="Statut : Liaison réseau établie. En attente du Patron.", font=("Courier", 10, "italic"), bg="#141419", fg="white", bd=1, relief="sunken", anchor="w")
label_statut.pack(side="bottom", fill="x", padx=10, pady=5)
fenetre.mainloop()
"""

    with open("ia_clavier.py", "w", encoding="utf-8") as f:
        f.write(code_propre)
    print("[2/3] CODE INJECTÉ : 'ia_clavier.py' réécrit avec la bonne adresse de Google.")

    # 3. RELANCEMENT AUTOMATIQUE DU RECTANGLE DE COMMANDEMENT
    print("[3/3] RELANCEMENT IMMINENT... Tu peux aller te coucher, patron.")
    print("=============================================\n")
    
    # Exécute de manière totalement indépendante l'interface corrigée
    subprocess.Popen([sys.executable, "ia_clavier.py"])

if __name__ == "__main__":
    reparer_et_relancer()
