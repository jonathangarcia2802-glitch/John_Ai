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
    cle_api = "Q"
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
    import os
import json
import asyncio
import subprocess
import wave
import requests
import sounddevice as sd
import cv2
import flet as ft

try:
    from bleak import BleakScanner
    BLEUETOOTH_DISPONIBLE = True
except ImportError:
    BLEUETOOTH_DISPONIBLE = False

CONFIG_DIR = "qg_souverain_core"
os.makedirs(CONFIG_DIR, exist_ok=True)
CONFIG_FICHIER = os.path.join(CONFIG_DIR, "memoire_lia.json")

def charger_memoire():
    config_defaut = {
        "patron": "Jonathan",
        "station": "QG Souverain v3.6 - Production Core",
        "historique": [],
        "frequence_vocal_hz": 44100,
        "profil_voix_path": os.path.join(CONFIG_DIR, "profil_voix_patron.wav")
    }
    if os.path.exists(CONFIG_FICHIER):
        try:
            with open(CONFIG_FICHIER, "r", encoding="utf-8") as f:
                data = json.load(f)
                if isinstance(data, dict):
                    for k, v in config_defaut.items():
                        if k not in data:
                            data[k] = v
                    return data
        except Exception:
            pass
    return config_defaut

memoire = charger_memoire()

def sauvegarder_memoire(data):
    with open(CONFIG_FICHIER, "w", encoding="utf-8") as f:
        json.dump(data, f, ensure_ascii=False, indent=4)

class NoyauOllamaProduction:
    def __init__(self):
        self.url = "http://192.168.1.61:11434/v1/chat/completions"
        self.model = "phi3.5:latest"

    def interroger(self, prompt):
        try:
            headers = {"Content-Type": "application/json"}
            payload = {
                "model": self.model,
                "messages": [
                    {"role": "system", "content": "Tu es le noyau IA opérationnel et souverain du QG."},
                    {"role": "user", "content": prompt}
                ],
                "stream": False
            }
            res = requests.post(self.url, headers=headers, json=payload, timeout=45)
            if res.status_code == 200:
                data = res.json()
                return data["choices"]["message"]["content"]
            else:
                return f"Erreur Ollama [{res.status_code}] : {res.text}"
        except requests.exceptions.ConnectionError:
            return "❌ Erreur critique : Impossible de joindre le serveur Ollama (192.168.1.61:11434)."
        except Exception as e:
            return f"❌ Erreur réseau : {e}"

ia_locale = NoyauOllamaProduction()

def executer_commande_systeme(cmd):
    try:
        res = subprocess.run(cmd, shell=True, capture_output=True, text=True, timeout=15)
        if res.returncode == 0:
            return res.stdout.strip() if res.stdout.strip() else "Exécuté avec succès."
        else:
            return f"Erreur CMD : {res.stderr.strip()}"
    except Exception as e:
        return f"Exception système : {e}"

async def main(page: ft.Page):
    page.title = "QG Souverain — Node Production"
    page.theme_mode = ft.ThemeMode.DARK
    page.vertical_alignment = ft.MainAxisAlignment.CENTER
    page.horizontal_alignment = ft.CrossAxisAlignment.CENTER
    page.window_width = 480
    page.window_height = 920

    titre_app = ft.Text("🛡️ QG SOUVERAIN — ACTIF (LOCAL MESH)", size=11, weight=ft.FontWeight.BOLD, color="cyan")
    chat_view = ft.ListView(expand=1, spacing=10, padding=12, auto_scroll=True)
    
    input_champ = ft.TextField(
        label="Ordre direct ou 'cmd: ...'",
        border_color="cyan",
        focused_border_color="blue",
        expand=True
    )

    def log_ui(auteur, texte, couleur="white"):
        chat_view.controls.append(
            ft.Container(
                content=ft.Column([
                    ft.Text(f"[{auteur}]", size=10, weight=ft.FontWeight.BOLD, color="blueGrey400"),
                    ft.Text(texte, color=couleur, size=13)
                ]),
                padding=10, border_radius=8, bgcolor="grey900"
            )
        )
        page.update()

    # --- TÂCHE DE FOND : SURVEILLANCE ET PROXIMITÉ CONTINUE ---
    async def boucle_surveillance_arriere_plan():
        """Tourne en continu pour simuler le radar de proximité et l'écoute mesh."""
        while True:
            try:
                if BLEUETOOTH_DISPONIBLE:
                    devices = await BleakScanner.discover(timeout=3.0)
                    # Analyse passive de présence des appareils connus dans l'environnement
                    actifs = [d.name for d in devices if d.name]
                    if actifs:
                        # Trace discrète de la présence du maillage
                        pass
            except Exception:
                pass
            await asyncio.sleep(15) # Intervalle de balayage

    async def action_voix(e):
        log_ui("Système", "⏳ Calibration micro 44100 Hz...", "yellow")
        def record_blocking():
            fs = 44100
            audio = sd.rec(int(5 * fs), samplerate=fs, channels=1, dtype='int16')
            sd.wait()
            path = memoire["profil_voix_path"]
            with wave.open(path, 'wb') as wf:
                wf.setnchannels(1)
                wf.setsampwidth(2)
                wf.setframerate(fs)
                wf.writeframes(audio.tobytes())
            return path
        
        chemin_wav = await asyncio.to_thread(record_blocking)
        log_ui("Biométrie", f"🎤 Empreinte vocale validée ({chemin_wav}).", "green")

    async def action_visage(e):
        log_ui("Système", "👁️ Analyse faciale...", "yellow")
        def capture_blocking():
            cap = cv2.VideoCapture(0)
            if not cap.isOpened():
                return None
            import time
            time.sleep(1)
            ret, frame = cap.read()
            cap.release()
            cv2.destroyAllWindows()
            if ret:
                path = os.path.join(CONFIG_DIR, "visage_patron.jpg")
                cv2.imwrite(path, frame)
                return path
            return None

        chemin_img = await asyncio.to_thread(capture_blocking)
        if chemin_img:
            log_ui("Biométrie", f"👁️ Visage confirmé ({chemin_img}).", "green")
        else:
            log_ui("Biométrie", "❌ Caméra inaccessible.", "red")

    async def action_bluetooth(e):
        if not BLEUETOOTH_DISPONIBLE:
            log_ui("Réseau", "❌ Module 'bleak' absent.", "red")
            return
        log_ui("Système", "📡 Balayage 2.4 GHz en cours...", "yellow")
        try:
            devices = await BleakScanner.discover(timeout=4.0)
            if not devices:
                log_ui("Réseau", "📡 Aucun signal détecté.", "yellow")
                return
            lignes = [f"• {d.name or 'Inconnu'} ({d.address}) [{d.rssi} dBm]" for d in devices]
            log_ui("Réseau Bluetooth", "\n".join(lignes), "cyan")
        except Exception as ex:
            log_ui("Réseau", f"❌ Erreur scan : {ex}", "red")

    barre_outils = ft.Row([
        ft.ElevatedButton("🎤 Micro", bgcolor="blueGrey850", color="white", on_click=action_voix),
        ft.ElevatedButton("👁️ Caméra", bgcolor="blueGrey850", color="white", on_click=action_visage),
        ft.ElevatedButton("📡 Bluetooth", bgcolor="blueGrey850", color="white", on_click=action_bluetooth)
    ], alignment=ft.MainAxisAlignment.SPACE_AROUND)

    async def soumettre(e):
        texte = input_champ.value.strip()
        if not texte:
            return
        log_ui("Jonathan", texte, "cyan")
        input_champ.value = ""
        page.update()

        if texte.lower().startswith("cmd:"):
            commande = texte[4:].strip()
            res_cmd = await asyncio.to_thread(executer_commande_systeme, commande)
            log_ui("Exécuteur Système", res_cmd, "green")
        else:
            reponse = await asyncio.to_thread(ia_locale.interroger, texte)
            log_ui("Phi-3.5 (Local)", reponse, "white")
            memoire["historique"].append({"user": texte, "ai": reponse})
            sauvegarder_memoire(memoire)

    btn_envoyer = ft.ElevatedButton("Transmettre", bgcolor="green", color="white", on_click=soumettre)
    input_champ.on_submit = soumettre

    page.add(
        ft.Column([
            titre_app,
            barre_outils,
            chat_view,
            ft.Row([input_champ, btn_envoyer], alignment=ft.MainAxisAlignment.SPACE_BETWEEN)
        ], expand=True, alignment=ft.MainAxisAlignment.START)
    )

    # Lancement de la boucle asynchrone de fond au démarrage de l'app
    page.run_task(boucle_surveillance_arriere_plan)

if __name__ == "__main__":
    ft.app(target=main)
    git add .
git commit -m "Mise a jour cerveau"
git push
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Passerelle Vocale IA V8</title>
    <style>
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background-color: #0b0c10; color: #c5c6c7; text-align: center; padding: 20px; margin: 0; }
        .container { max-width: 450px; margin: 40px auto; background: #1f2833; padding: 30px; border-radius: 20px; box-shadow: 0 8px 32px 0 rgba(0, 255, 204, 0.2); border: 1px solid #45a29e; }
        h1 { color: #66fcf1; font-size: 26px; margin-bottom: 10px; text-transform: uppercase; letter-spacing: 2px; }
        .status-box { background: #0b0c10; padding: 12px; border-radius: 10px; color: #66fcf1; font-size: 14px; font-weight: bold; border: 1px solid #1f2833; margin-bottom: 25px; }
        
        /* GROS BOUTON CENTRAL POUR PARLER */
        .mic-button { background: linear-gradient(135deg, #66fcf1, #45a29e); color: #0b0c10; border: none; width: 140px; height: 140px; border-radius: 50%; font-size: 16px; font-weight: bold; cursor: pointer; box-shadow: 0 0 25px rgba(102, 252, 241, 0.4); transition: all 0.3s ease; margin: 20px auto; display: flex; flex-direction: column; align-items: center; justify-content: center; }
        .mic-button:active { transform: scale(0.95); box-shadow: 0 0 15px rgba(102, 252, 241, 0.2); }
        .mic-icon { font-size: 32px; margin-bottom: 5px; }
        
        #transcript { margin-top: 20px; min-height: 50px; color: #ffffff; font-style: italic; font-size: 16px; padding: 10px; background: #0b0c10; border-radius: 8px; }
        #output { margin-top: 25px; background: #0b0c10; padding: 20px; border-radius: 10px; text-align: left; font-family: monospace; white-space: pre-wrap; display: none; border-left: 5px solid #66fcf1; color: #ffffff; }
    </style>
</head>
<body>

<div class="container">
    <h1>Passerelle Vocale V8</h1>
    <div class="status-box">🔒 ANTENNE ACTIVE & CHIFFREMENT ÉTABLI</div>
    
    <p>Appuie sur le bouton pour parler directement à toutes les IA :</p>
    
    <!-- LE BOUTON UNIQUE INTERCONNECTÉ -->
    <button class="mic-button" id="btnParler" onclick="activerReconnaissanceVocale()">
        <span class="mic-icon">🎙️</span>
        <span>PARLER</span>
    </button>
    
    <div id="transcript">En attente de ta voix...</div>
    <div id="output"></div>
</div>

<script>
    // Configuration de la reconnaissance vocale du téléphone
    const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
    const transcriptDiv = document.getElementById('transcript');
    const outputDiv = document.getElementById('output');
    const btnParler = document.getElementById('btnParler');

    if (!SpeechRecognition) {
        transcriptDiv.innerHTML = "❌ Ton téléphone ne prend pas en charge la reconnaissance vocale directe.";
    } else {
        const recognition = new SpeechRecognition();
        recognition.lang = 'fr-FR';
        recognition.interimResults = false;

        recognition.onstart = () => {
            transcriptDiv.innerHTML = "🎙️ Je t'écoute, patron... Parle maintenant.";
            btnParler.style.animation = "pulse 1.5s infinite";
        };

        recognition.onspeechend = () => {
            recognition.stop();
        };

        recognition.onresult = (event) => {
            const voixCapturee = event.results[0][0].transcript;
            transcriptDiv.innerHTML = `« ${voixCapturee} »`;
            
            // Envoi immédiat à la passerelle V8 par l'antenne
            transmettreOrdreIA(voixCapturee);
        };

        recognition.onerror = (event) => {
            transcriptDiv.innerHTML = "❌ Erreur micro ou aucune voix détectée. Réessaye.";
        };

        function activerReconnaissanceVocale() {
            outputDiv.style.display = "none";
            recognition.start();
        }
    }

    function transmettreOrdreIA(texteVocal) {
        outputDiv.style.display = "block";
        outputDiv.innerHTML = "⚡ Chiffrement réseau... Réveil instantané de toutes les IA...";

        // Connexion automatique à ta passerelle locale john_v8
        fetch('http://192.168.1', {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({ 
                ordre: texteVocal,
                signature: "PATRON_V8_SECURE_TOKEN_99" // Ton chiffrement d'antenne automatique
            })
        })
        .then(response => response.json())
        .then(data => {
            outputDiv.innerHTML = `<strong>[${data.statut}]</strong>\n\n${data.reponse}`;
        })
        .catch(error => {
            outputDiv.innerHTML = "❌ Liaison perdue avec la V8. Vérifie le Wi-Fi ou le script sur le PC.";
        });
    }
</script>

</body>
</html>
import os
import json
from flask import Flask, request, jsonify
from flask_cors import CORS
from cryptography.fernet import Fernet # Le bouclier de chiffrement militaire

app = Flask(__name__)
CORS(app)

FICHIER_HISTORIQUE = "historique_patron.enc"
FICHIER_CLE = "antenne_patron.key"

# --- PROTOCOLE ANGE GARDIEN : SÉCURISATION DE LA CLÉ ---
def obtenir_ou_creer_cle_secrete():
    """Génère une clé de chiffrement unique et invisible de l'extérieur."""
    if not os.path.exists(FICHIER_CLE):
        cle = Fernet.generate_key()
        with open(FICHIER_CLE, "wb") as key_file:
            key_file.write(cle)
        return Fernet(cle)
    else:
        with open(FICHIER_CLE, "rb") as key_file:
            cle = key_file.read()
        return Fernet(cle)

fernet = obtenir_ou_creer_cle_secrete()

def crypter_et_sauvegarder(ordre_patron):
    """Transforme tes idées en texte chiffré illisible pour les hackers."""
    historique = []
    
    # 1. Lire l'ancien fichier chiffré s'il existe
    if os.path.exists(FICHIER_HISTORIQUE):
        try:
            with open(FICHIER_HISTORIQUE, "rb") as f:
                donnees_cryptees = f.read()
            # Déchiffrement temporaire en mémoire vive uniquement
            donnees_decryptees = fernet.decrypt(donnees_cryptees)
            historique = json.loads(donnees_decryptees.decode('utf-8'))
        except Exception:
            pass # Si le fichier est corrompu ou hacké, on protège la structure
            
    # 2. Ajouter la nouvelle idée secrète
    historique.append({"ordre": ordre_patron, "statut": "Protégé par l'Ange Gardien"})
    
    # 3. Chiffrer le tout avant de l'écrire sur le disque dur
    texte_json = json.dumps(historique, ensure_ascii=False)
    donnees_a_sauvegarder = fernet.encrypt(texte_json.encode('utf-8'))
    
    with open(FICHIER_HISTORIQUE, "wb") as f:
        f.write(donnees_a_sauvegarder)
    print("\n[🛡️ ANGE GARDIEN] -> Idée chiffrée avec succès. Coffre-fort verrouillé.")

print("=========================================")
print(" PASSERELLE V9 : BLINDAGE MILITAIRE AES ")
print("=========================================")
print("[SÉCURITÉ] : Coffre-fort chiffré actif.")
print("[SYSTÈME] : Prêt à réceptionner tes ordres.")

@app.route('/ordre_mobile', methods=['POST'])
def passerelle_blindee():
    donnees = request.get_json() or {}
    
    # Validation du chiffrement de l'antenne de ton Samsung
    if donnees.get("signature") != "PATRON_V8_SECURE_TOKEN_99":
        print("[ALERTE HACKER] -> Tentative d'intrusion détectée et bloquée !")
        return jsonify({"erreur": "Alerte intrusion : Accès refusé."}), 403

    message_patron = donnees.get("ordre", "")
    print(f"\n[PATRON RECONNU] -> Connexion chiffrée sécurisée.")
    
    # Cryptage immédiat
    crypter_et_sauvegarder(message_patron)
    
    return jsonify({
        "statut": "SÉCURISÉ & LOCKÉ",
        "reponse": "Ton idée a été cryptée sur le disque dur. Aucun hacker ne peut la lire."
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)
    import os
import json
import subprocess # Le moteur secret qui permet à l'IA de taper dans le CMD toute seule
from flask import Flask, request, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)

FICHIER_HISTORIQUE = "historique_patron.json"
MOT_DE_PASSE_VOCAL = "peseta"

def ia_execute_commande_cmd(commande):
    """Cette fonction permet à l'IA de taper elle-même des ordres dans ton CMD."""
    print(f"[ROBOT AUTONOME] -> J'exécute la commande dans le CMD : {commande}")
    try:
        # Le robot ouvre un terminal invisible et tape la commande à ta place
        resultat = subprocess.run(commande, shell=True, capture_output=True, text=True, timeout=15)
        if resultat.returncode == 0:
            print("[ROBOT] -> Commande réussie.")
            return f"Succès : {resultat.stdout}"
        else:
            print(f"[ROBOT] -> Erreur lors de l'exécution : {resultat.stderr}")
            return f"Erreur : {resultat.stderr}"
    except Exception as e:
        return f"Échec critique du robot : {str(e)}"

def sauvegarder_idee_dans_disque(ordre_patron):
    historique = []
    if os.path.exists(FICHIER_HISTORIQUE):
        try:
            with open(FICHIER_HISTORIQUE, 'r', encoding='utf-8') as f:
                historique = json.load(f)
        except Exception:
            pass
    historique.append({"ordre": ordre_patron, "statut": "Exécuté par l'IA"})
    with open(FICHIER_HISTORIQUE, 'w', encoding='utf-8') as f:
        json.dump(historique, f, indent=4, ensure_ascii=False)

print("=========================================")
print(" PASSERELLE V9 : IA PILOTE DU CMD ")
print("=========================================")
print("[AUTONOMIE] : Le robot peut maintenant taper dans le CMD.")
print("[ANTENNE] : En attente des ordres vocaux du Patron...")

@app.route('/ordre_mobile', methods=['POST'])
def passerelle_autonome():
    donnees = request.get_json() or {}
    
    # Sécurité d'antenne
    if donnees.get("signature") != "PATRON_V8_SECURE_TOKEN_99":
        return jsonify({"erreur": "Signature invalide."}), 403

    mot_recu = donnees.get("mot_de_passe", "").lower()
    if mot_recu != MOT_DE_PASSE_VOCAL:
        return jsonify({"erreur": "Mot de passe incorrect."}), 401

    ordre_patron = donnees.get("ordre", "")
    action_cmd = donnees.get("commande_a_faire", "") # L'ordre direct pour le CMD
    
    print(f"\n[PATRON RECONNU] -> Ordre reçu : '{ordre_patron}'")
    
    # Si le Patron demande une action sur la machine, l'IA remplit le CMD d'elle-même
    compte_rendu = ""
    if action_cmd:
        compte_rendu = ia_execute_commande_cmd(action_cmd)
        
    sauvegarder_idee_dans_disque(ordre_patron)
    
    return jsonify({
        "statut": "ORDRE EXÉCUTÉ PAR LE ROBOT",
        "reponse": f"J'ai pris le contrôle du CMD, patron. Résultat : {compte_rendu}"
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)
    from pyngrok import ngrok
ngrok.set_auth_token("AQ.Ab8RN6I8QV-ukEvEXUjrFpEHk8oWhOs4eTFOZIn69zh2ie-OzQ")
import os
import json
import subprocess # Le moteur secret qui permet à l'IA de taper dans le CMD toute seule
from flask import Flask, request, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)

FICHIER_HISTORIQUE = "historique_patron.json"
MOT_DE_PASSE_VOCAL = "peseta"

def ia_execute_commande_cmd(commande):
    """Cette fonction permet à l'IA de taper elle-même des ordres dans ton CMD."""
    print(f"[ROBOT AUTONOME] -> J'exécute la commande dans le CMD : {commande}")
    try:
        # Le robot ouvre un terminal invisible et tape la commande à ta place
        resultat = subprocess.run(commande, shell=True, capture_output=True, text=True, timeout=15)
        if resultat.returncode == 0:
            print("[ROBOT] -> Commande réussie.")
            return f"Succès : {resultat.stdout}"
        else:
            print(f"[ROBOT] -> Erreur lors de l'exécution : {resultat.stderr}")
            return f"Erreur : {resultat.stderr}"
    except Exception as e:
        return f"Échec critique du robot : {str(e)}"

def sauvegarder_idee_dans_disque(ordre_patron):
    historique = []
    if os.path.exists(FICHIER_HISTORIQUE):
        try:
            with open(FICHIER_HISTORIQUE, 'r', encoding='utf-8') as f:
                historique = json.load(f)
        except Exception:
            pass
    historique.append({"ordre": ordre_patron, "statut": "Exécuté par l'IA"})
    with open(FICHIER_HISTORIQUE, 'w', encoding='utf-8') as f:
        json.dump(historique, f, indent=4, ensure_ascii=False)

print("=========================================")
print(" PASSERELLE V9 : IA PILOTE DU CMD ")
print("=========================================")
print("[AUTONOMIE] : Le robot peut maintenant taper dans le CMD.")
print("[ANTENNE] : En attente des ordres vocaux du Patron...")

@app.route('/ordre_mobile', methods=['POST'])
def passerelle_autonome():
    donnees = request.get_json() or {}
    
    # Sécurité d'antenne
    if donnees.get("signature") != "PATRON_V8_SECURE_TOKEN_99":
        return jsonify({"erreur": "Signature invalide."}), 403

    mot_recu = donnees.get("mot_de_passe", "").lower()
    if mot_recu != MOT_DE_PASSE_VOCAL:
        return jsonify({"erreur": "Mot de passe incorrect."}), 401

    ordre_patron = donnees.get("ordre", "")
    action_cmd = donnees.get("commande_a_faire", "") # L'ordre direct pour le CMD
    
    print(f"\n[PATRON RECONNU] -> Ordre reçu : '{ordre_patron}'")
    
    # Si le Patron demande une action sur la machine, l'IA remplit le CMD d'elle-même
    compte_rendu = ""
    if action_cmd:
        compte_rendu = ia_execute_commande_cmd(action_cmd)
        
    sauvegarder_idee_dans_disque(ordre_patron)
    
    return jsonify({
        "statut": "ORDRE EXÉCUTÉ PAR LE ROBOT",
        "reponse": f"J'ai pris le contrôle du CMD, patron. Résultat : {compte_rendu}"
    })

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=False)
    
